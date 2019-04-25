
# StructureMap

Inherits from: [NameableArtefact](../Base/NameableArtefact.md)



## Description

Links a source and target structure where there is a semantic equivalence between the source and the target structures.


## Attributes

**isExtension** (*bool*): Whether this map is an extension.

**alias** (*string*): An alternate identification of the map, that allows the relation of multiple maps to be expressed by the sharing of this value.

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.

### Inherited



## References

### Inherited

**map** ([ComponentMap](ComponentMap.md) - 1..*): Association to the ComponentMap.
**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.
**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.
**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description


## Referenced By

[StructureSet](StructureSet.md) (as map)


