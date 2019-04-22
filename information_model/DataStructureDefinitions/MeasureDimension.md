
# MeasureDimension

Inherits from: [Dimension](Dimension.md)



A statistical concept that identifies the component in the key structure that has an enumerated list of measures. This dimension has, as its representation the ConceptScheme that enumerates the measure Concepts.

## Attributes

id: string

uri: Url

urn: Urn



## References

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

conceptIdentity: [Concept](../ConceptSchemes/Concept.md) (One) - No description

localRepresentation: [Representation](../Base/Representation.md) (One) - No description

role: [Concept](../ConceptSchemes/Concept.md) (ZeroOrMany) - Association to the Concept that specifies the role that the Dimension plays in the DataStructureDefinition.




