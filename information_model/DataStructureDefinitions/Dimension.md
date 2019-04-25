
# Dimension

Inherits from: [Component](../Base/Component.md)

## Subclasses

[MeasureDimension](MeasureDimension.md)

[TimeDimension](TimeDimension.md)



## Description

A metadata concept used (most probably together with other metadata concepts) to classify a statistical series, e.g. a statistical concept indicating a certain economic activity or a geographical reference area.


## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.

### Inherited



## References

**role** ([Concept](../ConceptSchemes/Concept.md) - 0..*): Association to the Concept that specifies the role that the Dimension plays in the DataStructureDefinition.

### Inherited

**conceptIdentity** ([Concept](../ConceptSchemes/Concept.md) - 1): No description
**localRepresentation** ([Representation](../Base/Representation.md) - 1): No description
**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description


## Referenced By

[DimensionDescriptor](DimensionDescriptor.md) (as components)

[GroupDimensionDescriptor](GroupDimensionDescriptor.md) (as components)

[DimensionRelationship](DimensionRelationship.md) (as dimensions)

[KeyValue](KeyValue.md) (as valueFor)

[MeasureKeyValue](MeasureKeyValue.md) (as valueFor)

[TimeKeyValue](TimeKeyValue.md) (as valueFor)

[CodedKeyValue](CodedKeyValue.md) (as valueFor)

[UncodedKeyValue](UncodedKeyValue.md) (as valueFor)


