
# ComponentList

Inherits from: [](..//.md)

## Subclasses

[DimensionDescriptor](../DataStructureDefinitions/DimensionDescriptor.md)

[AttributeDescriptor](../DataStructureDefinitions/AttributeDescriptor.md)

[MeasureDescriptor](../DataStructureDefinitions/MeasureDescriptor.md)

[GroupDimensionDescriptor](../DataStructureDefinitions/GroupDimensionDescriptor.md)

[MetadataTarget](../MetadataStructureDefinitions/MetadataTarget.md)

[ReportStructure](../MetadataStructureDefinitions/ReportStructure.md)



An abstract definition of a list of components. A concrete example is a DimensionDescriptor which defines the list of Dimensions in a DataStructureDefinition.



## References

components: [Component](Component.md) (OneOrMany) - An aggregate association to one or more components which make up the list.



## Referenced By

[Structure](Structure.md) (as grouping)

[Structure](Structure.md) (as grouping)

[MetadataTargetRegion](../Constraints/MetadataTargetRegion.md) (as componentList)


