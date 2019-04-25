
# SeriesKey

Inherits from: [Key](Key.md)



## Description

Comprises the cross product of values of all the KeyValues that, together with the KeyValue of the observationDimension identify uniquely an Observation.




## References

describedBy: [GroupDimensionDescriptor](GroupDimensionDescriptor.md) (One) - Associates the DimensionDescriptor defined in the DataStructureDefinition.

contains: [Observation](Observation.md) (OneOrMany) - Observations contained by this SeriesKey.

keyValues: [KeyValue](KeyValue.md) (OneOrMany) - Association to the individual KeyValues that comprise the Key.

attachedAttribute: [AttributeValue](AttributeValue.md) (ZeroOrMany) - Association to the AttributeValues relating to the Series Key or Group Key.




