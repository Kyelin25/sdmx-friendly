
# DataSetTarget

Inherits from: [TargetObject](TargetObject.md)



## Description

The target object is a DataSet.


## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

conceptIdentity: [Concept](../ConceptSchemes/Concept.md) (One) - An association to the Concept which carries the values of the measures.

localRepresentation: [Representation](../Base/Representation.md) (One) - Associates a Representation to the TargetObject that must be respected when the object is identified in any MetadataSet. This may be enumerated or non-enumerated.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description




