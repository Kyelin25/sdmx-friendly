
# Component

Inherits from: [IdentifiableArtefact](IdentifiableArtefact.md)

## Subclasses

[Dimension](../DataStructureDefinitions/Dimension.md)

[DataAttribute](../DataStructureDefinitions/DataAttribute.md)

[PrimaryMeasure](../DataStructureDefinitions/PrimaryMeasure.md)

[TargetObject](../MetadataStructureDefinitions/TargetObject.md)

[MetadataAttribute](../MetadataStructureDefinitions/MetadataAttribute.md)



## Description

A component is an abstract super class used to define qualitative and quantitative data and metadata items that belong to a ComponentList and hence a Structure. Component is refined through its sub-classes.


## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.

### Inherited



## References

### Inherited

**conceptIdentity** ([Concept](../ConceptSchemes/Concept.md) - 1): No description
**localRepresentation** ([Representation](Representation.md) - 1): No description
**contains** ([Annotation](Annotation.md) - 0..*): No description


## Referenced By

[ComponentMap](../StructureMaps/ComponentMap.md) (as source)

[ComponentMap](../StructureMaps/ComponentMap.md) (as target)

[ComponentList](ComponentList.md) (as components)

[ComponentValue](../MetadataStructureDefinitions/ComponentValue.md) (as valueFor)

[MemberSelection](../Constraints/MemberSelection.md) (as valuesFor)


