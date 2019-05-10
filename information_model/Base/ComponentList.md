
# ComponentList

*Abstract*



## Subclasses

[DimensionDescriptor](../DataStructure/DimensionDescriptor.md)

[AttributeDescriptor](../DataStructure/AttributeDescriptor.md)

[MeasureDescriptor](../DataStructure/MeasureDescriptor.md)

[GroupDimensionDescriptor](../DataStructure/GroupDimensionDescriptor.md)

[MetadataTarget](../MetadataStructure/MetadataTarget.md)

[ReportStructure](../MetadataStructure/ReportStructure.md)



## Description

An abstract definition of a list of components. A concrete example is a DimensionDescriptor which defines the list of Dimensions in a DataStructureDefinition.




## References

**components** ([Component](Component.md) - 1..*): An aggregate association to one or more components which make up the list.

### Inherited



## Referenced By

[Structure](Structure.md) (as grouping)

[DataStructureDefinition](../DataStructure/DataStructureDefinition.md) (as grouping)

[MetadataTargetRegion](../Registry/MetadataTargetRegion.md) (as componentList)


