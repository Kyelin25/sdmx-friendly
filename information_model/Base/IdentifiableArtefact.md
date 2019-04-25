
# IdentifiableArtefact

Inherits from: [AnnotableArtefact](AnnotableArtefact.md)

## Subclasses

[NameableArtefact](NameableArtefact.md)

[Component](Component.md)

[HierarchicalCode](../HierarchicalCodelists/HierarchicalCode.md)

[Transition](../Process/Transition.md)



## Description

Provides identity to all derived classes. It also provides Annotations to derived classes because it is a subclass of AnnotableArtefact


## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

**contains** ([Annotation](Annotation.md) - 0..*): No description



## Referenced By

[Categorisation](../CategorySchemes/Categorisation.md) (as categorisedArtefact)

[ProcessArtefact](../Process/ProcessArtefact.md) (as artefact)


