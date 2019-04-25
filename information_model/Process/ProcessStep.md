
# ProcessStep





## Description

A specific operation, performed on data or metadata in order to validate or to derive new information according to a given set of rules.




## References

input: [ProcessArtefact](ProcessArtefact.md) (ZeroOrMany) - Association to the ProcessArtefact that identifies the objects which are input to the ProcessStep.

output: [ProcessArtefact](ProcessArtefact.md) (ZeroOrMany) - Association to the ProcessArtefact that identifies the objects which are output from the ProcessStep.

computation: [Computation](Computation.md) (ZeroOrOne) - Association to one or more Computations.

transition: [Transition](Transition.md) (ZeroOrMany) - Association to one or more Transitions.

child: [ProcessStep](ProcessStep.md) (ZeroOrMany) - Association to child ProcessSteps that combine to form a part of this ProcessStep.



## Referenced By

[Process](Process.md) (as step)

[Transition](Transition.md) (as target)

[ProcessStep](ProcessStep.md) (as child)


