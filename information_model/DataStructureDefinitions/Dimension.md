
# Dimension

Inherits from: [Component](../Base/Component.md)

## Subclasses

[MeasureDimension](MeasureDimension.md)

[TimeDimension](TimeDimension.md)



A metadata concept used (most probably together with other metadata concepts) to classify a statistical series, e.g. a statistical concept indicating a certain economic activity or a geographical reference area.

## Attributes

id: string

uri: Url

urn: Urn



## References

role: [Concept](../ConceptSchemes/Concept.md) (ZeroOrMany) - Association to the Concept that specifies the role that the Dimension plays in the DataStructureDefinition.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

conceptIdentity: [Concept](../ConceptSchemes/Concept.md) (One) - No description

localRepresentation: [Representation](../Base/Representation.md) (One) - No description



## Referenced By

[ComponentList](../Base/ComponentList.md) (as components)

[ComponentList](../Base/ComponentList.md) (as components)

[DimensionRelationship](DimensionRelationship.md) (as dimensions)

[KeyValue](KeyValue.md) (as valueFor)

[KeyValue](KeyValue.md) (as valueFor)

[KeyValue](KeyValue.md) (as valueFor)

[KeyValue](KeyValue.md) (as valueFor)

[KeyValue](KeyValue.md) (as valueFor)


