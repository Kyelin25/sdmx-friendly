
# DataAttribute

Inherits from: [Component](../Base/Component.md)

## Subclasses

[ReportingYearStartDay](ReportingYearStartDay.md)



A characteristic of an object or entity.

## Attributes

usageStatus: UsageStatus

id: string

uri: Url

urn: Urn



## References

role: [Concept](../ConceptSchemes/Concept.md) (ZeroOrMany) - Association to the Concept that specifies the role that the DataAttribute plays in the DataStructureDefinition.

relatedTo: [AttributeRelationship](AttributeRelationship.md) (One) - Association to an AttributeRelationship.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

conceptIdentity: [Concept](../ConceptSchemes/Concept.md) (One) - No description

localRepresentation: [Representation](../Base/Representation.md) (One) - No description



## Referenced By

[ComponentList](../Base/ComponentList.md) (as components)

[AttributeValue](AttributeValue.md) (as valueFor)

[AttributeValue](AttributeValue.md) (as valueFor)

[AttributeValue](AttributeValue.md) (as valueFor)


