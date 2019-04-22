
# MetadataAttribute

Inherits from: [Component](../Base/Component.md)



Identifies a Concept for which a value may be reported in a MetadataSet.

## Attributes

isPresentational: bool

minOccurs: int

maxOccurs: int

id: string

uri: Url

urn: Urn



## References

child: [MetadataAttribute](MetadataAttribute.md) (ZeroOrMany) - A child of this MetadataAttribute.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

conceptIdentity: [Concept](../ConceptSchemes/Concept.md) (One) - An association to the Concept which defines the semantic of the attribute.

localRepresentation: [Representation](../Base/Representation.md) (One) - No description



## Referenced By

[MetadataAttribute](MetadataAttribute.md) (as child)

[ComponentList](../Base/ComponentList.md) (as components)

[ReportedAttribute](ReportedAttribute.md) (as valueFor)

[ReportedAttribute](ReportedAttribute.md) (as valueFor)

[ReportedAttribute](ReportedAttribute.md) (as valueFor)

[ReportedAttribute](ReportedAttribute.md) (as valueFor)

[ReportedAttribute](ReportedAttribute.md) (as valueFor)

[ReportedAttribute](ReportedAttribute.md) (as valueFor)


