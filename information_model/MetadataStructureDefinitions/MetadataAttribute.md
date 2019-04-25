
# MetadataAttribute

Inherits from: [Component](../Base/Component.md)



## Description

Identifies a Concept for which a value may be reported in a MetadataSet.


## Attributes

**isPresentational** (*bool*): Indication that the MetadataAttribute is present for structural purposes (i.e. it has child attributes) and that no value for this attribute is expected to be reported in a MetadataSet using this ReportStructure.

**minOccurs** (*int*): Specifies how many occurrences of the MetadataAttribute may be reported at this point in the MetadataReport.

**maxOccurs** (*int*): Specifies how many occurrences of the MetadataAttribute may be reported at this point in the MetadataReport.

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.

### Inherited



## References

**child** ([MetadataAttribute](MetadataAttribute.md) - 0..*): A child of this MetadataAttribute.

### Inherited

**conceptIdentity** ([Concept](../ConceptSchemes/Concept.md) - 1): An association to the Concept which defines the semantic of the attribute.
**localRepresentation** ([Representation](../Base/Representation.md) - 1): Associates a Representation to the TargetObject that must be respected when the object is identified in any MetadataSet. This may be enumerated or non-enumerated.
**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description


## Referenced By

[MetadataAttribute](MetadataAttribute.md) (as child)

[ReportStructure](ReportStructure.md) (as components)

[ReportedAttribute](ReportedAttribute.md) (as valueFor)

[NonEnumeratedAttributeValue](NonEnumeratedAttributeValue.md) (as valueFor)

[XHTMLAttributeValue](XHTMLAttributeValue.md) (as valueFor)

[TextAttributeValue](TextAttributeValue.md) (as valueFor)

[OtherNonEnumeratedAttributeValue](OtherNonEnumeratedAttributeValue.md) (as valueFor)

[EnumeratedAttributeValue](EnumeratedAttributeValue.md) (as valueFor)


