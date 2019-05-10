
# Component

*Abstract*

Inherits from: [IdentifiableArtefact](IdentifiableArtefact.md)

## Subclasses

[Dimension](../DataStructure/Dimension.md)

[DataAttribute](../DataStructure/DataAttribute.md)

[PrimaryMeasure](../DataStructure/PrimaryMeasure.md)

[TargetObject](../MetadataStructure/TargetObject.md)

[MetadataAttribute](../MetadataStructure/MetadataAttribute.md)



## Description

A component is an abstract super class used to define qualitative and quantitative data and metadata items that belong to a ComponentList and hence a Structure. Component is refined through its sub-classes.


## Attributes

### Inherited

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

**conceptIdentity** ([Concept](../ConceptScheme/Concept.md) - 1): No description

**localRepresentation** ([Representation](Representation.md) - 1): No description

### Inherited

**contains** ([Annotation](Annotation.md) - 0..*): No description



## Referenced By

[ComponentMap](../Mapping/ComponentMap.md) (as source)

[ComponentMap](../Mapping/ComponentMap.md) (as target)

[ComponentList](ComponentList.md) (as components)

[ComponentValue](../MetadataStructure/ComponentValue.md) (as valueFor)

[MemberSelection](../Registry/MemberSelection.md) (as valuesFor)


