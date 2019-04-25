
# Transition

Inherits from: [IdentifiableArtefact](../Base/IdentifiableArtefact.md)



## Description

An expression in a textual or formalised way of the transformation of data between two specific operations (Processes) performed on the data.


## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

target: [ProcessStep](ProcessStep.md) (One) - Associates the ProcessStep that is the target of the Transition.

condition: [InternationalString](../Base/InternationalString.md) (One) - Associates a textual description of the Transition.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[ProcessStep](ProcessStep.md) (as transition)


