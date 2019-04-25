
# DataAttribute

Inherits from: [Component](../Base/Component.md)

## Subclasses

[ReportingYearStartDay](ReportingYearStartDay.md)



## Description

A characteristic of an object or entity.


## Attributes

**usageStatus** (*UsageStatus*): Defines the usage status which is constrained by the data type UsageStatus.

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.

### Inherited



## References

### Inherited

**role** ([Concept](../ConceptSchemes/Concept.md) - 0..*): Association to the Concept that specifies the role that the DataAttribute plays in the DataStructureDefinition.
**relatedTo** ([AttributeRelationship](AttributeRelationship.md) - 1): Association to an AttributeRelationship.
**conceptIdentity** ([Concept](../ConceptSchemes/Concept.md) - 1): No description
**localRepresentation** ([Representation](../Base/Representation.md) - 1): No description
**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description


## Referenced By

[AttributeDescriptor](AttributeDescriptor.md) (as components)

[AttributeValue](AttributeValue.md) (as valueFor)

[UncodedAttributeValue](UncodedAttributeValue.md) (as valueFor)

[CodedAttributeValue](CodedAttributeValue.md) (as valueFor)


