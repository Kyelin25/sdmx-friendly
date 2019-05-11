
# DimensionComponent

*Abstract*

Inherits from: [Component](../Base/Component.md)

## Subclasses

[Dimension](Dimension.md)

[MeasureDimension](MeasureDimension.md)

[TimeDimension](TimeDimension.md)



## Description

Abstract class providing a base for Dimension, TimeDimension and MeasureDimension.


## Attributes

### Inherited

**order** (*int*): The order in which the DimensionComponent appears in the DataStructureDefinition.

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

**role** ([Concept](../ConceptScheme/Concept.md) - 0..*): Association to the Concept that specifies the role that the Dimension plays in the DataStructureDefinition.

### Inherited

**conceptIdentity** ([Concept](../ConceptScheme/Concept.md) - 1): No description

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


