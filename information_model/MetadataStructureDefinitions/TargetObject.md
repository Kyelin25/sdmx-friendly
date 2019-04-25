
# TargetObject

Inherits from: [Component](../Base/Component.md)

## Subclasses

[DimensionDescriptorValuesTarget](DimensionDescriptorValuesTarget.md)

[IdentifiableObjectTarget](IdentifiableObjectTarget.md)

[DataSetTarget](DataSetTarget.md)

[ReportPeriodTarget](ReportPeriodTarget.md)

[ConstraintTarget](ConstraintTarget.md)





## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.

### Inherited



## References

**conceptIdentity** ([Concept](../ConceptSchemes/Concept.md) - 1): An association to the Concept which carries the values of the measures.

**localRepresentation** ([Representation](../Base/Representation.md) - 1): Associates a Representation to the TargetObject that must be respected when the object is identified in any MetadataSet. This may be enumerated or non-enumerated.

**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description

### Inherited



## Referenced By

[MetadataTarget](MetadataTarget.md) (as components)

[TargetObjectValue](TargetObjectValue.md) (as valueFor)

[TargetDataKey](TargetDataKey.md) (as valueFor)

[TargetIdentifiableObject](TargetIdentifiableObject.md) (as valueFor)

[TargetDataSet](TargetDataSet.md) (as valueFor)

[TargetReportPeriod](TargetReportPeriod.md) (as valueFor)


