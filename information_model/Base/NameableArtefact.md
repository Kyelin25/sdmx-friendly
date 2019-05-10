
# NameableArtefact

*Abstract*

Inherits from: [IdentifiableArtefact](IdentifiableArtefact.md)

## Subclasses

[VersionableArtefact](VersionableArtefact.md)

[Item](Item.md)

[MetadataSet](../MetadataStructure/MetadataSet.md)

[Level](../Codelist/Level.md)

[Hierarchy](../Codelist/Hierarchy.md)

[ItemSchemeMap](../Mapping/ItemSchemeMap.md)

[HybridCodelistMap](../Mapping/HybridCodelistMap.md)

[StructureMap](../Mapping/StructureMap.md)



## Description

Provides a name and description to all derived classes in addition to identification and Annotations.


## Attributes

### Inherited

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

**name** ([InternationalString](InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

### Inherited

**contains** ([Annotation](Annotation.md) - 0..*): No description




