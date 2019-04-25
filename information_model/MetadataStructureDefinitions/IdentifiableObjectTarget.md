
# IdentifiableObjectTarget

Inherits from: [TargetObject](TargetObject.md)



## Description

The target object is a specified object type.


## Attributes

**objectType** (*IdentifiableObjectType*): Identifies the object type.

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.

### Inherited



## References

### Inherited

**conceptIdentity** ([Concept](../ConceptSchemes/Concept.md) - 1): An association to the Concept which carries the values of the measures.
**localRepresentation** ([Representation](../Base/Representation.md) - 1): Associates a Representation to the TargetObject that must be respected when the object is identified in any MetadataSet. This may be enumerated or non-enumerated.
**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description



