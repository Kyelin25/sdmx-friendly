
# Computation

Inherits from: [AnnotableArtefact](../Base/AnnotableArtefact.md)



## Description

Describes in textual form the computations involved in the process.


## Attributes

**localId** (*string*): Distinguishes between Computations in the same Process.

**softwarePackage** (*string*): Together with softwareLanguage and softwareVersion provides information about the software that is used to perform the Computation.

**softwareLanguage** (*string*): Together with softwarePackage and softwareVersion provides information about the software that is used to perform the Computation.

**softwareVersion** (*string*): Together with softwarePackage and softwareLanguage provides information about the software that is used to perform the Computation.

### Inherited



## References

**description** ([InternationalString](../Base/InternationalString.md) - 1..*): Text describing of giving additional information about the Computation. This can be in multiple language variants.

### Inherited

**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description


## Referenced By

[ProcessStep](ProcessStep.md) (as computation)


