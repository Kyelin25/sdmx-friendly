
# MeasureDimension



Inherits from: [DimensionComponent](DimensionComponent.md)



## Description

A statistical concept that identifies the component in the key structure that has an enumerated list of measures. This dimension has, as its representation the ConceptScheme that enumerates the measure Concepts.


## Attributes

### Inherited

**order** (*int*): The order in which the DimensionComponent appears in the DataStructureDefinition.

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

### Inherited

**role** ([Concept](../ConceptScheme/Concept.md) - 0..*): Association to the Concept that specifies the role that the Dimension plays in the DataStructureDefinition.

**conceptIdentity** ([Concept](../ConceptScheme/Concept.md) - 1): No description

**localRepresentation** ([Representation](../Base/Representation.md) - 1): No description

**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description




