
# Representation





## Description

The allowable value or format for Component or Concept.




## References

**enumerated** ([ItemScheme](ItemScheme.md) - 0..1): Association to an enumerated list that contains the allowable content for the Component when reported in a DataSet or MetadataSet. The type of enumerated list that is allowed for any concrete Component is shown in the constraints on the association (e.g. IdentifierComponent can have any of the sub-classes of ItemScheme, whereas MeasureDimension must have a ConceptScheme).

**nonEnumerated** ([Facet](Facet.md) - 0..*): Association to a set of Facets that define the allowable format for the content of the Component when reported in a DataSet or MetadataSet.

**nonEnumerated** ([ExtendedFacet](ExtendedFacet.md) - 0..*): Association to a set of Facets that define the allowable format for the content of the Component when reported in a DataSet or MetadataSet.

### Inherited



## Referenced By

[Concept](../ConceptSchemes/Concept.md) (as coreRepresentation)

[Component](Component.md) (as localRepresentation)

[Dimension](../DataStructureDefinitions/Dimension.md) (as localRepresentation)

[MeasureDimension](../DataStructureDefinitions/MeasureDimension.md) (as localRepresentation)

[TimeDimension](../DataStructureDefinitions/TimeDimension.md) (as localRepresentation)

[DataAttribute](../DataStructureDefinitions/DataAttribute.md) (as localRepresentation)

[ReportingYearStartDay](../DataStructureDefinitions/ReportingYearStartDay.md) (as localRepresentation)

[PrimaryMeasure](../DataStructureDefinitions/PrimaryMeasure.md) (as localRepresentation)

[TargetObject](../MetadataStructureDefinitions/TargetObject.md) (as localRepresentation)

[DimensionDescriptorValuesTarget](../MetadataStructureDefinitions/DimensionDescriptorValuesTarget.md) (as localRepresentation)

[IdentifiableObjectTarget](../MetadataStructureDefinitions/IdentifiableObjectTarget.md) (as localRepresentation)

[DataSetTarget](../MetadataStructureDefinitions/DataSetTarget.md) (as localRepresentation)

[ReportPeriodTarget](../MetadataStructureDefinitions/ReportPeriodTarget.md) (as localRepresentation)

[ConstraintTarget](../MetadataStructureDefinitions/ConstraintTarget.md) (as localRepresentation)

[MetadataAttribute](../MetadataStructureDefinitions/MetadataAttribute.md) (as localRepresentation)

[ConceptUsage](../MetadataStructureDefinitions/ConceptUsage.md) (as localRepresentation)


