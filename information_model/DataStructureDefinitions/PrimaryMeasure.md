
# PrimaryMeasure

Inherits from: [Component](../Base/Component.md)



## Description

The metadata concept that is the phenomenon to be measured in a data set. In a data set the instance of the measure is often called the observation.


## Attributes

id: string

uri: Url

urn: Urn



## References

conceptIdentity: [Concept](../ConceptSchemes/Concept.md) (One) - An association to the Concept which carries the values of the measures.

localRepresentation: [Representation](../Base/Representation.md) (One) - No description

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[MeasureDescriptor](MeasureDescriptor.md) (as components)

[Observation](Observation.md) (as valueFor)


