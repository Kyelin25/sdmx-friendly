# Dimension
[Definition](../../information_model/DataStructure/TimeDimension.md)

## Description

The TimeDimension is exactly what it says on the tin. It is a dimension of a DataStructureDefinition wholly concerned with the measurement of time, whether that be points in time or time periods. Each DataStructureDefinition **may** have one TimeDimension. It does not **need** to have one. 

A TimeDimension may refer to a Concept (just like Dimension and MeasureDimension) that gives it meaning. This is called the *conceptIdentity*. I'm not sure what, if anything, happens if you refer to an utterly non-time-related Concept like "Country of Birth" (that is, apart from confusing your users). Unlike Dimension and MeasureDimension, TimeDimension may not refer to a Concept as its *role* in the DSD, as it always plays the role of "time" (seems fair). Additionally, the TimeDimension must be have a non-enumerated Representation, and its FacetValueType must be a valid time FacetValueType (these are listed in the Notes). This may be the *coreRepresentation* of the TimeDimension's *conceptIdentity* Concept (as long as it's a valid non-enumerated Representation) or the *localRepresentation* declared with the TimeDimension.

You might be thinking that everything TimeDimension can do, you can do with a Dimension. You could set its *role* to "Time" and take a valid time FacetValueType as its Representation. However, by making the TimeDimension its own type, it makes it possible to treat it differently to other dimensions. Concretely, there are wildly different rules for querying based on Dimensions and MeasureDimensions, and querying on the TimeDimension. For example, querying an SDMX REST API provides the "startPeriod" and "endPeriod" query parameters to define a range of times.

## Examples
The most common use of the TimeDimension is simply to allow all "observationalTimePeriod" values. This is a meta-FacetValueType that contains all other time-related FacetValueTypes. In other words, it's open slather:
```javascript
{
    "id": "TIME_PERIOD",
    "conceptIdentity": "urn:sdmx:org.sdmx.infomodel.conceptscheme.Concept=ABS:CS_COMMON(1.0.0).TIME_PERIOD"
    "representation":
    {
        "textFormat":
        {
            "facetValueType": "observationalTimePeriod"
        }
    }
}
```
However, it's possible to use a more restrictive FacetValueType. For example, perhaps we are releasing a monthly survey, and so only have datapoints for each month:
```javascript
{
    "id": "TIME_PERIOD",
    "conceptIdentity": "urn:sdmx:org.sdmx.infomodel.conceptscheme.Concept=ABS:CS_COMMON(1.0.0).TIME_PERIOD"
    "representation":
    {
        {
            "textFormat": 
            {
                "facetValueType": "reportingQuarter"
            }
        }
    }
}
```

## Notes

Although in the model I can't find anything constraining the choice of *id* for the TimeDimension, in the SDMX-ML implementation of SDMX at least, the *id* of the TimeDimension is always "TIME_PERIOD". I suspect this will be the case in all implementations.

I believe it's possible to constrain the TimeDimension's Representation even further than just selecting a restrictive FacetValueType, by providing FacetValues to do something like specify a time-range. However, I'm not confident enough of how to do so to put it in here. See the [explanation of Facets](../Base/Facets.md) for more information on how this might work.

## Identification

 The TimeDimension is not a MaintainableArtefact. It may only be identified through its DataStructureDefinitions using the following pattern:
 ```
    urn:sdmx:org.sdmx.infomodel.datastructure.Dimension={AgencyIdChain}:{DataStructureDefinitionId}({DataStructureDefinitionVersion}).{TimeDimensionId}
 ```

 For example, if we were to assume that the TimeDimension used in the Examples section belonged to the DSD ABS:LFS(1.0.0), it would have the identification:
 ```
    urn:sdmx:org.sdmx.infomodel.datastructure.TimeDimension=ABS:LFS(1.0.0).TIME_PERIOD
 ```

 For those paying close attention, yes, TimeDimension is actually contained in a DimensionDescriptor, which would imply that its *id* should be used in the URN for the TimeDimension. However, because there is only ever one DimensionDescriptor in a DSD, it is omitted from the URN.