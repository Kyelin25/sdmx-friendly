
# DataAttribute

Inherits from: [Component](../Base/Component.md)

## Subclasses

[ReportingYearStartDay](ReportingYearStartDay.md)



## Description

A characteristic of an object or entity.


## Attributes

usageStatus: UsageStatus

id: string

uri: Url

urn: Urn



## References

role: [Concept](../ConceptSchemes/Concept.md) (ZeroOrMany) - Association to the Concept that specifies the role that the DataAttribute plays in the DataStructureDefinition.

relatedTo: [AttributeRelationship](AttributeRelationship.md) (One) - Association to an AttributeRelationship.

conceptIdentity: [Concept](../ConceptSchemes/Concept.md) (One) - No description

localRepresentation: [Representation](../Base/Representation.md) (One) - No description

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[AttributeDescriptor](AttributeDescriptor.md) (as components)

[AttributeValue](AttributeValue.md) (as valueFor)

[UncodedAttributeValue](UncodedAttributeValue.md) (as valueFor)

[CodedAttributeValue](CodedAttributeValue.md) (as valueFor)


