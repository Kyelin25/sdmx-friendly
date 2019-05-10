# ConceptScheme and Concept
[ConceptScheme Definition](../../information_model/ConceptScheme/ConceptScheme.md) [Concept Definition](../../information_model/ConceptScheme/Concept.md)

## Description

The Concept is one of the most fundamental (and in my opinion confusing) parts of the SDMX standard. Whenever I try describe what a Concept is I end up using words like "thing", "concept, but with a small c" and "idea". Concepts exist in SDMX to give **meaning** to other things, like Dimensions and Attributes. By reusing them, you can encode the idea (dammit) that certain objects have semantic equivalence. For example, if two Dimensions in two different DataStructureDefinitions both take meaning from the same Concept, it's not insane to think they are equivalent in some way.

Concepts are Nameable, and hence must be given an *id* (as all Nameables are Identifiable) of some sort, as well as a multi-lingual name. They may optionally be given a multi-lingual description. Like Codes, it's good practice to make the *id* semi-meaningful so that glancing at it gives some meaning.

In addition to the above, Concepts are allowed to have a *coreRepresentation*. This is a [Representation](../../information_model/Base/Representation.md) to provide as a default, when no other is provided. That is, when something that needs a Representation refers to the Concept to give it meaning (like a Dimension taking meaning from a Concept), unless otherwise specified, the Concept's *coreRepresentation* will be used. The *coreRepresentation* is inherited by child Concepts (see next paragraph for Concept hierarchies). See [Representation Explananation](../Base/Representation.md) for an explanation of how Representations work. This doesn't just make it easier to define Dimensions and DataAttributes and their ilk (because you don't need to specify a Representation if you're just using the default), but it makes it more likely that other data modellers in your organization will use the appropriate Codelist (or non-enumerated Representation... but most of the time it'll be a Codelist) for their Dimensions.

Concepts are maintained in ConceptSchemes, where their parent-child hierarchy (inherited from Item) can be used to show semantic links between Concepts. For example, you might have the following parent-child chain of Concepts.
- Country
    - Country of Birth
        - Country of Birth of Person
        - Country of Birth of Mother
        - Country of Birth of Father

You can see how Country of Birth is a more specific case of Country, and Country of Birth of Person is a more specific case of Country of Birth. There's nothing forcing you to maintain a hierarchy like this. You could equally have a flat ConceptScheme with the same Concepts in it, you just lose any sense of a hierarchy.

## Best Practice

- Concept ids should be semi-descriptive and in all capitals
- Prepend "CS_" to the beginning of ConceptScheme ids so it's clear if anybody sees it on its own they're looking at a ConceptScheme
-  Reuse existing ConceptSchemes and Concepts where possible. Check the [Global SDMX Registry](https://registry.sdmx.org) to see if there is already a globally-recognized ConceptScheme that does what you want. If not, perhaps you can at least reuse some of the Concepts
- Try to reuse Concepts throughout your model when possible, to enable greater discoverability and comparability

## Examples

For a ConceptScheme containing Concepts mainly to do with Country of Birth, you might have the following:
```javascript
{
    "id": "CS_COUNTRY_CONCEPTS",
    "agencyId": "ABS",
    "version": "1.0.0",
    "name": [{"en", "Country-related Concepts"}],
    "description": [{"en", "Concepts relating to country and uses of country, such as Country of Birth"}],
    "concepts":[
        {
            "id": "COUNTRY",
            "name": [{"en", "Country"}],
            "description": [{"en", "A region that is identified as a distinct entity in political geography"}],
            "representation": {
                "enumeration": "urn:sdmx:org.sdmx.infomodel.codelist.Codelist=ABS:CL_COUNTRY(1.0.0)"
            },
            "concepts":[
                {
                    {
                        "id": "COB",
                        "name": [{"en", "Country of Birth"}],
                        "concepts":[
                            {
                                "id": "COB_PERSON",
                                "name": [{"en", "Country of Birth of Person"}],
                                "description": [{"en", "The country in which a person was born."}]
                            },
                            {
                                "id":"COB_MOTHER",
                                "name":[{"en", "Country of Birth of Mother"}],
                                "description": [{"en", "The country in which a person's mother was born."}]
                            },
                            {
                                "id": "COB_FATHER",
                                "name": [{"en", "Country of Birth of Father"}],
                                "description": [{"en", "The country in which a person's father was born."}]
                            }
                        ]
                    }
                }
            ]
        }
    ]
}
```
 You can see here that by nesting COB underneath COUNTRY, and COB_PERSON, COB_MOTHER and COB_FATHER underneath COB, we provide a level of semantic equivalence between them. Additionally, by doing so, we ensure that the use of the CL_COUNTRY Codelist as the default representation for country-based Concepts applies to all of these Concepts. If we were to use any of these in a DSD to provide meaning to a Dimension, it would use that Codelist by default. 

 ## Notes

 Like [Codes in Codelists](../Codelist/CodelistAndCode.md#Notes), Concepts in ConceptSchemes are not stored in a hierarchy, despite having one. This means that Concepts must have unique *ids* within their entire ConceptScheme, as their ancestors are not taken into account when identifying them (meaning duplicate *ids* would lead to ambiguity).

 ## Identification

 Identification of a ConceptScheme works just like any other MaintainableArtefact (see [IdentifiableArtefact](../Base/IdentifiableArtefact.md) for details).

As mentioned in the Notes section, Concepts are not stored in hierarchy. This means a Concepts's parent Concepts are ignored when identifying it as per the rules laid out in the [IdentifiableArtefact](../Base/IdentifiableArtefact.md) explanation. So a Concept is always identified like so:
```
    urn:sdmx:org.sdmx.infomodel.conceptscheme.Concept={AgencyIdChain}:{ConceptSchemeId}({ConceptSchemeVersion}).{ConceptId}
```

For example, identifying the COB_PARENT (a child of COB, itself a child of COUNTRY) in the ConceptScheme used in the Examples section would look like:
```
    urn:sdmx:org.sdmx.infomodel.conceptscheme.Concept=ABS:CS_COUNTRY_CONCEPTS(1.0.0).COB_PARENT
```