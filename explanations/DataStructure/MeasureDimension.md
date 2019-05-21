# Dimension
[Definition](../../information_model/DataStructure/TimeDimension.md)

## Description

The MeasureDimension is a strange beast. Certainly to me it's the most confusing of the dimensions in a DataStructureDefinition. Just like the other two types ([Dimension](Dimension.md) and [TimeDimension](TimeDimension.md)), it serves to uniquely identify an observation. However, its function is to tell you something about **what** is being measured, something referred to variously as a measure, or data item, or just "value". 

I think an example is in order, to try describe this better. Say you take a survey. You collect the age and sex of participants, in order to classify them in your output, and you also ask them their income. You group them into age-ranges and for each age-range and sex combination you calculate the mean income and median income, then release those figures. In this example, your age-ranges and sex variables are pretty obviously Dimensions.... they serve to classify the released values. However, "mean income" and "median income" are actually measures. By encoding these as values of a MeasureDimension you represent that these are separate data items that you're disseminating, not just different ways of classifying your data (you also get some extra bonuses that we'll discuss in a second).

So, how do we represent a MeasureDimension? Well, unlike a Dimension, MeasureDimensions can't use a non-enumerated [Representation](../Base/Representation.md). In fact, they can't even use a Codelist in their Representation. MeasureDimensions are restricted to referring to a ConceptScheme as an enumerated Representation. We'll explain why we'd do that in a second, but it's worth highlighting that because the *coreRepresentation* of a Concept can't be a ConceptScheme, this means that the MeasureDimension must always specify an explicit *localRepresentation*.

Why refer to a ConceptScheme? In my mind there's two main reasons. Firstly, by making the values of the MeasureDimension Concepts, we can give semantic meaning to the measures the MeasureDimension represents, much as Concepts give semantic meaning to Dimensions or DataAttributes. The second reason has to do with how the MeasureDimension interacts with the [PrimaryMeasure](PrimaryMeasure.md). I don't want to go into too much detail here, but essentially the PrimaryMeasure is the actual value stored in observations. "But wait, I thought that's what the MeasureDimension was for?" I hear you say. Exactly! The MeasureDimension overrules the PrimaryMeasure in two key ways:
- The Representation of the selected Concept in the MeasureDimension over-rules the semantic of the Concept referred to by the PrimaryMeasure
- The *coreRepresentation* of the selected Concept in the MeasureDimension Representation over-rules the Representation in use by the PrimaryMeasure
The first point is just a re-phrasing of giving semantic meaning to our measures. However, the second means that we can represent measures in one DSD that are wildly different. For example, one might be expressed as a decimal, the other as an integer. Without referring to a ConceptScheme in the MeasureDimension's Representation, we'd have no way of specifying these different Representations.

Now, you're not obliged to have a MeasureDimension. Firstly, you might only actually have one measure **in** your data, and so the [PrimaryMeasure](PrimaryMeasure.md) will do the trick. Secondly, you might decide you want to go the old-school route, and encode your "measures" as a normal Dimension (usually with the *id* "MEASURE") and just settle for losing the semantic meaning and different Representations.

We've mostly focussed on the Representation of the MeasureDimension, largely because that's the area in which it most differs from the Dimension. However, it's worth highlighting that like a Dimension, a MeasureDimension requires an *id*, and takes its semantic and name from a *conceptIdentity* reference to a Concept, and may optionally play a role in the DSD based on a *role* reference to a Concept. However, I've never seen a MeasureDimension that doesn't just have something like "Measure" as its *conceptIdentity* and I struggle to think what *role* you would give it. See [Dimension](Dimension.md) for a description of *conceptIdentity* and *role*.

## Examples

Let's express the survey example above by outlining first the ConceptScheme we're going to use for our MeasureDimension and then the MeasureDimension itself.
```javascript
{
    "id": "CS_SURVEY_MEASURES",
    "agencyId": "ABS",
    "version": "1.0.0",
    "name": [{"en", "Measure Concepts"}]
    "concepts":[
        {
            "id": "INCOME_MEDIAN",
            "name": [{"en", "Median Income"}],
            "representation": {
                "textFormat":
                {
                    "facetValueType": "integer"
                }
            }
        },
        {
            "id": "INCOME_MEAN",
            "name": [{"en", "Mean Income"}],
            "representation": {
                "textFormat":
                {
                    "facetValueType": "decimal"
                }
            }
        }
    ]
}
```
Let's look at the ConceptScheme before we move onto the MeasureDimension itself. Note that each of the Concepts has a Representation defined. Note that "Median Income" must be an integer, but "Mean Income" can be any decimal. This is one of the advantages of using a MeasureDimension. Okay, now for the MeasureDimension itself.
```javascript
{
    "id": "MEASURE",
    "conceptIdentity": "urn:sdmx:org.sdmx.infomodel.conceptscheme.Concept=ABS:CS_SURVEY_CONCEPTS(1.0.0).MEASURE"
    "localRepresentation": {
        "enumeration": "urn:sdmx:org.sdmx.infomodel.conceptscheme.ConceptScheme=ABS:CS_SURVEY_MEASURES(1.0.0)"
    }
}
```
Here we define the MeasureDimension. Note that although we've given it the *id* "MEASURE", we didn't need to. It could really have any *id*, as the fact that it's a MeasureDimension artefact is enough to tell us that it's a measure.

## Notes

As stated in the Description section, MeasureDimensions are constrained in their choice of Representations. Non-enumerated Representations are **not** allowed, and enumerated Representations that refer to ConceptSchemes are allowed. You must always specify a *localRepresentation* for a MeasureDimension (as the *coreRepresentation* of a Concept can never be a ConceptScheme so cannot be inherited by the MeasureDimension).

It's worth highlighting that just like Dimension, MeasureDimension is **not** a subclass of NameableArtefact and so does **not** get its own name. The name of the MeasureDimension comes from its *conceptIdentity*.

The *coreRepresentation* of any Concept in the MeasureDimension's ConceptScheme must be compatible with the PrimaryMeasure's Representation. In practice this should mean it's either the same, or more restrictive. For example, if the PrimaryMeasure is represented as a decimal, the *coreRepresentation* could be an integer, but the opposite would not be valid.

Although MeasureDimensions are IdentifiableArtefacts and thus require an *id*, in the SDMX-ML implementation of SDMX (and likely others), if none is explicitly provided, it's assumed that the *id* of the MeasureDimension is the *id* of the *conceptIdentity*. Unlike Dimensions, you should never run into problems with duplicate *ids*, because there's only ever one MeasuerDimension in a DSD. However, it's worth making sure that this doesn't cause problems with web-service queries.

## Identification

 MeasureDimensions are not MaintainableArtefacts. They may only be identified through their DataStructureDefinitions using the following pattern:
 ```
    urn:sdmx:org.sdmx.infomodel.datastructure.MeasureDimension={AgencyIdChain}:{DataStructureDefinitionId}({DataStructureDefinitionVersion}).{MeasureDimensionId}
 ```

 For example, if we were to assume that the MeasureDimension used in the Examples section belonged to the DSD ABS:INCOME_SURVEY(1.0.0), it would have the identification:
 ```
    urn:sdmx:org.sdmx.infomodel.datastructure.MeasureDimension=ABS:INCOME_SURVEY(1.0.0).MEASURE
 ```

 For those paying close attention, yes, MeasureDimensions are actually contained in a DimensionDescriptor, which would imply that its *id* should be used in the URN for a MeasureDimension. However, because there is only ever one DimensionDescriptor in a DSD, it is omitted from the URN.