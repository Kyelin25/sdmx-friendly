
# Computation

Inherits from: [AnnotableArtefact](../Base/AnnotableArtefact.md)



## Description

Describes in textual form the computations involved in the process.


## Attributes

localId: string

softwarePackage: Together with softwareLanguage and softwareVersion provides information about the software that is used to perform the Computation.

softwareLanguage: string

softwareVersion: string



## References

description: [InternationalString](../Base/InternationalString.md) (OneOrMany) - Text describing of giving additional information about the Computation. This can be in multiple language variants.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[ProcessStep](ProcessStep.md) (as computation)


