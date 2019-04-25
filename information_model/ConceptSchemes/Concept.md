
# Concept

Inherits from: [Item](../Base/Item.md)



## Description

A concept is a unit of knowledge created by a unique combination of characteristics.


## Attributes

### Inherited

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

**coreRepresentation** ([Representation](../Base/Representation.md) - 0..1): Associates a Representation.

**ISOConcept** ([ISOConcept](ISOConcept.md) - 0..1): Association to an ISO concept reference.

### Inherited

**child** ([Concept](Concept.md) - 0..*): A child of this Concept

**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description



## Referenced By

[ConceptScheme](ConceptScheme.md) (as items)

[Concept](Concept.md) (as child)

[Component](../Base/Component.md) (as conceptIdentity)

[Dimension](../DataStructureDefinitions/Dimension.md) (as role)

[Dimension](../DataStructureDefinitions/Dimension.md) (as conceptIdentity)

[MeasureDimension](../DataStructureDefinitions/MeasureDimension.md) (as role)

[MeasureDimension](../DataStructureDefinitions/MeasureDimension.md) (as conceptIdentity)

[TimeDimension](../DataStructureDefinitions/TimeDimension.md) (as role)

[TimeDimension](../DataStructureDefinitions/TimeDimension.md) (as conceptIdentity)

[DataAttribute](../DataStructureDefinitions/DataAttribute.md) (as role)

[DataAttribute](../DataStructureDefinitions/DataAttribute.md) (as conceptIdentity)

[ReportingYearStartDay](../DataStructureDefinitions/ReportingYearStartDay.md) (as role)

[ReportingYearStartDay](../DataStructureDefinitions/ReportingYearStartDay.md) (as conceptIdentity)

[PrimaryMeasure](../DataStructureDefinitions/PrimaryMeasure.md) (as conceptIdentity)

[TargetObject](../MetadataStructureDefinitions/TargetObject.md) (as conceptIdentity)

[DimensionDescriptorValuesTarget](../MetadataStructureDefinitions/DimensionDescriptorValuesTarget.md) (as conceptIdentity)

[IdentifiableObjectTarget](../MetadataStructureDefinitions/IdentifiableObjectTarget.md) (as conceptIdentity)

[DataSetTarget](../MetadataStructureDefinitions/DataSetTarget.md) (as conceptIdentity)

[ReportPeriodTarget](../MetadataStructureDefinitions/ReportPeriodTarget.md) (as conceptIdentity)

[ConstraintTarget](../MetadataStructureDefinitions/ConstraintTarget.md) (as conceptIdentity)

[MetadataAttribute](../MetadataStructureDefinitions/MetadataAttribute.md) (as conceptIdentity)

[ConceptMap](../ItemSchemeMaps/ConceptMap.md) (as source)

[ConceptMap](../ItemSchemeMaps/ConceptMap.md) (as target)

[MeasureKeyValue](../DataStructureDefinitions/MeasureKeyValue.md) (as value)

[ConceptUsage](../MetadataStructureDefinitions/ConceptUsage.md) (as concept)


