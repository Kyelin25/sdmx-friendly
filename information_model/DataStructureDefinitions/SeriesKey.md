
# SeriesKey

Inherits from: [Key](Key.md)



## Description

Comprises the cross product of values of all the KeyValues that, together with the KeyValue of the observationDimension identify uniquely an Observation.




## References

**describedBy** ([GroupDimensionDescriptor](GroupDimensionDescriptor.md) - 1): Associates the DimensionDescriptor defined in the DataStructureDefinition.

**contains** ([Observation](Observation.md) - 1..*): Observations contained by this SeriesKey.

**keyValues** ([KeyValue](KeyValue.md) - 1..*): Association to the individual KeyValues that comprise the Key.

**attachedAttribute** ([AttributeValue](AttributeValue.md) - 0..*): Association to the AttributeValues relating to the Series Key or Group Key.

### Inherited




