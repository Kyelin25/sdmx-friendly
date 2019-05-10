
# PrimaryMeasure



Inherits from: [Component](../Base/Component.md)



## Description

The metadata concept that is the phenomenon to be measured in a data set. In a data set the instance of the measure is often called the observation.


## Attributes

### Inherited

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

### Inherited

**conceptIdentity** ([Concept](../ConceptScheme/Concept.md) - 1): An association to the Concept which carries the values of the measures.

**localRepresentation** ([Representation](../Base/Representation.md) - 1): No description

**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description



## Referenced By

[MeasureDescriptor](MeasureDescriptor.md) (as components)

[Observation](Observation.md) (as valueFor)


