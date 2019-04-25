
# NameableArtefact

Inherits from: [IdentifiableArtefact](IdentifiableArtefact.md)

## Subclasses

[VersionableArtefact](VersionableArtefact.md)

[Item](Item.md)

[MetadataSet](../MetadataStructureDefinitions/MetadataSet.md)

[Level](../HierarchicalCodelists/Level.md)

[Hierarchy](../HierarchicalCodelists/Hierarchy.md)

[ItemSchemeMap](../ItemSchemeMaps/ItemSchemeMap.md)

[HybridCodelistMap](../HybridCodelistMap/HybridCodelistMap.md)

[StructureMap](../StructureMaps/StructureMap.md)



## Description

Provides a name and description to all derived classes in addition to identification and Annotations.


## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

name: [InternationalString](InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](Annotation.md) (ZeroOrMany) - No description




