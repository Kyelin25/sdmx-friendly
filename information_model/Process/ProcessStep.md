
# ProcessStep





## Description

A specific operation, performed on data or metadata in order to validate or to derive new information according to a given set of rules.




## References

**input** ([ProcessArtefact](ProcessArtefact.md) - 0..*): Association to the ProcessArtefact that identifies the objects which are input to the ProcessStep.

**output** ([ProcessArtefact](ProcessArtefact.md) - 0..*): Association to the ProcessArtefact that identifies the objects which are output from the ProcessStep.

**computation** ([Computation](Computation.md) - 0..1): Association to one or more Computations.

**transition** ([Transition](Transition.md) - 0..*): Association to one or more Transitions.

**child** ([ProcessStep](ProcessStep.md) - 0..*): Association to child ProcessSteps that combine to form a part of this ProcessStep.

### Inherited



## Referenced By

[Process](Process.md) (as step)

[Transition](Transition.md) (as target)

[ProcessStep](ProcessStep.md) (as child)


