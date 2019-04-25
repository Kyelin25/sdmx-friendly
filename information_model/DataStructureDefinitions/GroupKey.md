
# GroupKey

Inherits from: [Key](Key.md)



## Description

A set of KeyValues that comprise a partial key, of the same dimensionality as the TimeSeriesKey for the purpose of attaching DataAttributes.




## References

**describedBy** ([GroupDimensionDescriptor](GroupDimensionDescriptor.md) - 1): Associates the GroupDimensionDescriptor defined in the DataStructureDefinition.

**keyValues** ([KeyValue](KeyValue.md) - 1..*): Association to the individual KeyValues that comprise the Key.

**attachedAttribute** ([AttributeValue](AttributeValue.md) - 0..*): Association to the AttributeValues relating to the Series Key or Group Key.

**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description




