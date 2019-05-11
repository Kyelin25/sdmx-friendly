
# Representation







## Description

The allowable value or format for Component or Concept.




## References

**enumerated** ([ItemScheme](ItemScheme.md) - 0..1): Association to an enumerated list that contains the allowable content for the Component when reported in a DataSet or MetadataSet. The type of enumerated list that is allowed for any concrete Component is shown in the constraints on the association (e.g. IdentifierComponent can have any of the sub-classes of ItemScheme, whereas MeasureDimension must have a ConceptScheme).

**nonEnumerated** ([Facet](Facet.md) - 0..*): Association to a set of Facets that define the allowable format for the content of the Component when reported in a DataSet or MetadataSet.

**nonEnumerated** ([ExtendedFacet](ExtendedFacet.md) - 0..*): Association to a set of Facets that define the allowable format for the content of the Component when reported in a DataSet or MetadataSet.

### Inherited



## Referenced By

[Concept](../ConceptScheme/Concept.md) (as coreRepresentation)

[Component](Component.md) (as localRepresentation)

[DimensionComponent](../DataStructure/DimensionComponent.md) (as localRepresentation)

[Dimension](../DataStructure/Dimension.md) (as localRepresentation)

[MeasureDimension](../DataStructure/MeasureDimension.md) (as localRepresentation)

[TimeDimension](../DataStructure/TimeDimension.md) (as localRepresentation)

[DataAttribute](../DataStructure/DataAttribute.md) (as localRepresentation)

[ReportingYearStartDay](../DataStructure/ReportingYearStartDay.md) (as localRepresentation)

[PrimaryMeasure](../DataStructure/PrimaryMeasure.md) (as localRepresentation)

[TargetObject](../MetadataStructure/TargetObject.md) (as localRepresentation)

[DimensionDescriptorValuesTarget](../MetadataStructure/DimensionDescriptorValuesTarget.md) (as localRepresentation)

[IdentifiableObjectTarget](../MetadataStructure/IdentifiableObjectTarget.md) (as localRepresentation)

[DataSetTarget](../MetadataStructure/DataSetTarget.md) (as localRepresentation)

[ReportPeriodTarget](../MetadataStructure/ReportPeriodTarget.md) (as localRepresentation)

[ConstraintTarget](../MetadataStructure/ConstraintTarget.md) (as localRepresentation)

[MetadataAttribute](../MetadataStructure/MetadataAttribute.md) (as localRepresentation)

[ConceptUsage](../MetadataStructure/ConceptUsage.md) (as localRepresentation)


