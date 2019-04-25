
# TimeDimension

Inherits from: [Dimension](Dimension.md)



## Description

A metadata concept that identifies the component in the key structure that has the role of "time".


## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

role: [Concept](../ConceptSchemes/Concept.md) (ZeroOrMany) - Association to the Concept that specifies the role that the Dimension plays in the DataStructureDefinition.

conceptIdentity: [Concept](../ConceptSchemes/Concept.md) (One) - No description

localRepresentation: [Representation](../Base/Representation.md) (One) - No description

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description




