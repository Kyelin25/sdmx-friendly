
# PrimaryMeasure

Inherits from: [Component](../Base/Component.md)



The metadata concept that is the phenomenon to be measured in a data set. In a data set the instance of the measure is often called the observation.

## Attributes

id: string

uri: Url

urn: Urn



## References

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

conceptIdentity: [Concept](../ConceptSchemes/Concept.md) (One) - An association to the Concept which carries the values of the measures.

localRepresentation: [Representation](../Base/Representation.md) (One) - No description



## Referenced By

[ComponentList](../Base/ComponentList.md) (as components)

[Observation](Observation.md) (as valueFor)


