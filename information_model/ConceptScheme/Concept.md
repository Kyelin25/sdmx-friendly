
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

[DimensionComponent](../DataStructure/DimensionComponent.md) (as role)

[DimensionComponent](../DataStructure/DimensionComponent.md) (as conceptIdentity)

[Dimension](../DataStructure/Dimension.md) (as role)

[Dimension](../DataStructure/Dimension.md) (as conceptIdentity)

[MeasureDimension](../DataStructure/MeasureDimension.md) (as role)

[MeasureDimension](../DataStructure/MeasureDimension.md) (as conceptIdentity)

[TimeDimension](../DataStructure/TimeDimension.md) (as role)

[TimeDimension](../DataStructure/TimeDimension.md) (as conceptIdentity)

[DataAttribute](../DataStructure/DataAttribute.md) (as role)

[DataAttribute](../DataStructure/DataAttribute.md) (as conceptIdentity)

[ReportingYearStartDay](../DataStructure/ReportingYearStartDay.md) (as role)

[ReportingYearStartDay](../DataStructure/ReportingYearStartDay.md) (as conceptIdentity)

[PrimaryMeasure](../DataStructure/PrimaryMeasure.md) (as conceptIdentity)

[TargetObject](../MetadataStructure/TargetObject.md) (as conceptIdentity)

[DimensionDescriptorValuesTarget](../MetadataStructure/DimensionDescriptorValuesTarget.md) (as conceptIdentity)

[IdentifiableObjectTarget](../MetadataStructure/IdentifiableObjectTarget.md) (as conceptIdentity)

[DataSetTarget](../MetadataStructure/DataSetTarget.md) (as conceptIdentity)

[ReportPeriodTarget](../MetadataStructure/ReportPeriodTarget.md) (as conceptIdentity)

[ConstraintTarget](../MetadataStructure/ConstraintTarget.md) (as conceptIdentity)

[MetadataAttribute](../MetadataStructure/MetadataAttribute.md) (as conceptIdentity)

[ConceptMap](../Mapping/ConceptMap.md) (as source)

[ConceptMap](../Mapping/ConceptMap.md) (as target)

[MeasureKeyValue](../DataStructure/MeasureKeyValue.md) (as value)

[ConceptUsage](../MetadataStructure/ConceptUsage.md) (as concept)


