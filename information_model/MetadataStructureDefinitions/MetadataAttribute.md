
# MetadataAttribute

Inherits from: [Component](../Base/Component.md)



## Description

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

conceptIdentity: [Concept](../ConceptSchemes/Concept.md) (One) - An association to the Concept which defines the semantic of the attribute.

localRepresentation: [Representation](../Base/Representation.md) (One) - Associates a Representation to the TargetObject that must be respected when the object is identified in any MetadataSet. This may be enumerated or non-enumerated.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[MetadataAttribute](MetadataAttribute.md) (as child)

[ReportStructure](ReportStructure.md) (as components)

[ReportedAttribute](ReportedAttribute.md) (as valueFor)

[NonEnumeratedAttributeValue](NonEnumeratedAttributeValue.md) (as valueFor)

[XHTMLAttributeValue](XHTMLAttributeValue.md) (as valueFor)

[TextAttributeValue](TextAttributeValue.md) (as valueFor)

[OtherNonEnumeratedAttributeValue](OtherNonEnumeratedAttributeValue.md) (as valueFor)

[EnumeratedAttributeValue](EnumeratedAttributeValue.md) (as valueFor)


