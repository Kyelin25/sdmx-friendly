# Dimension
[Definition](../../information_model/DataStructure/Dimension.md)

## Description

Little 'd' dimensions identify observations. Concretely providing values for each of the set of Dimensions along with any TimeDimension or MeasureDimension are enough to uniquely identify any given observation in a DataSet. Like Concept, I struggle to provide a description for Dimension that doesn't boil down to handwaving or a bunch of examples. Luckily, anybody familiar with statistics will be familiar with the concept of dimensions, so really all I need to say is that Dimensions are exactly what you think they are.

When a Dimension is defined, it must be provided with an *id* (as it inherits from IdentifiableArtefact) and a reference to a Concept, named its *conceptIdentity*. This Concept provides the Dimension with its semantic meaning (and also its name!). For example, a Dimension describing ages would use an age-related Concept in order to express this. Similarly, a Dimension describing the country of birth of persons might link to a Concept named "Country of Birth of Person".

A Dimension also needs a Representation. This defines the values that can be provided for this Dimension in the data. Representations are explained in great detail [here](../Base/Representation.md). You may optionally specify a *localRepresentation* for the Dimension, or you may inherit the *coreRepresentation* of the *conceptIdentity* Concept. If the Concept doesn't have a *coreRepresentation* I assume this should result in an error (though I've never seen this happen). Dimensions may only have Codelist Representations or non-enumerated Representations. To constrain a Dimension to use a subset of the defined Representation, we use Constraints. I only mention this here to highlight that there's no direct way on the Dimension itself to do so.

In addition to referencing a Concept as the Dimension's *conceptIdentity*, you **may** reference another Concept as its *role*. This is used to provide additional information as to what role the Dimension is performing in the DataStructureDefinition. Think of a Dimension that lists the countries of the world. By applying the *role* Geography to it, you mark it as something that can be mapped. The intention is that the statistical community agrees on a series of shared Concepts that can be used to mark Dimensions as being usable for certain things. Then applications can be built to check the *role* of Dimensions and process them accordingly (like trying to map boundaries for Dimensions marked as Geographies).

## Examples

A Dimension describing the country of birth of persons could be created as follows:
```javascript
{
    "id": "COB",
    "conceptIdentity": "urn:sdmx:org.sdmx.infomodel.conceptscheme.Concept=ABS:CS_COUNTRY_CONCEPTS(1.0.0).COB"
}
```
In this example, we don't declare a *localRepresentation* and so inherit whatever has been defined as the *coreRepresentation* of the "COB" Concept. If, however, we wanted to use a different Representation, we might define it like so:
```javascript
{
    "id": "COB",
    "conceptIdentity": "urn:sdmx:org.sdmx.infomodel.conceptscheme.Concept=ABS:CS_COUNTRY_CONCEPTS(1.0.0).COB"
    "localRepresentation": {
        "enumeration": "urn:sdmx:org.sdmx.infomodel.codelist.Codelist=ABS:CL_ALTERNATE_COUNTRY(1.0.0)"
    },
}
```
To mark the "Country of Birth" Dimension as being mappable, we could use the *role* reference to refer to a "Geography" Concept:
```javascript
{
    "id": "COB",
    "conceptIdentity": "urn:sdmx:org.sdmx.infomodel.conceptscheme.Concept=ABS:CS_COUNTRY_CONCEPTS(1.0.0).COB"
    "role": "urn:sdmx:org.sdmx.infomodel.conceptscheme.Concept=SDMX:SDMX_CONCEPT_ROLES(1.0).GEO"
}
```

## Notes

As stated in the Description section, Dimensions are constrained in their choice of Representations. Non-enumerated Representations are allowed, and enumerated Representations that refer to Codelists are allowed.

It's worth highlighting that Dimension is **not** a subclass of NameableArtefact and so does **not** get its own name. The name of the Dimension comes from its *conceptIdentity*. This can be a problem if you have Dimensions in different DataStructureDefinitions that are in essence describing the same thing (and so ought to refer to the same Concept for comparability and discoverability) but you wish to have different display names for them.

Although Dimensions are IdentifiableArtefacts and thus require an *id*, in the SDMX-ML implementation of SDMX (and likely others), if none is explicitly provided, it's assumed that the *id* of the Dimension is the *id* of the *conceptIdentity*. Now, because the Dimensions need to be differentiated from one another by their *id*, if multiple Dimensions reference Concepts with the same *id* (even if they're different Concepts, in different ConceptSchemes), then at least one of them will need to have an explicit *id* provided.

 ## Identification

 Dimensions are not MaintainableArtefacts. They may only be identified through their DataStructureDefinitions using the following pattern:
 ```
    urn:sdmx:org.sdmx.infomodel.datastructure.Dimension={AgencyIdChain}:{DataStructureDefinitionId}({DataStructureDefinitionVersion}).{DimensionId}
 ```

 For example, if we were to assume that the Dimension used in the Examples section belonged to the DSD ABS:LFS(1.0.0), it would have the identification:
 ```
    urn:sdmx:org.sdmx.infomodel.datastructure.Dimension=ABS:LFS(1.0.0).COB
 ```

 For those paying close attention, yes, Dimensions are actually contained in a DimensionDescriptor, which would imply that its *id* should be used in the URN for a Dimension. However, because there is only ever one DimensionDescriptor in a DSD, it is omitted from the URN.