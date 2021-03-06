
# GroupDimensionDescriptor



Inherits from: [ComponentList](../Base/ComponentList.md)



## Description

A set of metadata concepts that define a partial key derived from the DimensionDescriptor in a DataStructureDefinition.




## References

**constraint** ([Constraint](../Registry/Constraint.md) - 0..1): Identifies an AttachmentConstraint that specifies the subset of Dimension, Measure or Attribute values to which an Attribute can be attached.

### Inherited

**components** ([DimensionComponent](DimensionComponent.md) - 0..*): An association to the Dimension and MeasureDimension components that comprise the group.



## Referenced By

[GroupKey](GroupKey.md) (as describedBy)

[SeriesKey](SeriesKey.md) (as describedBy)

[GroupRelationship](GroupRelationship.md) (as groupKey)

[DimensionRelationship](DimensionRelationship.md) (as groupKey)


