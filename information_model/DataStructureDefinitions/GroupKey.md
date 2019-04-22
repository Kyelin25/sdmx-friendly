
# GroupKey

Inherits from: [Key](Key.md)



A set of KeyValues that comprise a partial key, of the same dimensionality as the TimeSeriesKey for the purpose of attaching DataAttributes.



## References

describedBy: [GroupDimensionDescriptor](GroupDimensionDescriptor.md) (One) - Associates the GroupDimensionDescriptor defined in the DataStructureDefinition.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

keyValues: [KeyValue](KeyValue.md) (OneOrMany) - Association to the individual KeyValues that comprise the Key.

attachedAttribute: [AttributeValue](AttributeValue.md) (ZeroOrMany) - Association to the AttributeValues relating to the Series Key or Group Key.




