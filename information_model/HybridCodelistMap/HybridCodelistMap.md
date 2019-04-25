
# HybridCodelistMap

Inherits from: [NameableArtefact](../Base/NameableArtefact.md)



## Description

Associates a Codelist and a HierarchicalCodelist.


## Attributes

**alias** (*string*): An alternate identification of the map, that allows the relation of multiple maps to be expressed by the sharing of this value.

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

source: [SourceList](SourceList.md) (One) - Association to the source List.

target: [TargetList](TargetList.md) (One) - Associationg to the target List.

hybridCodeMap: [HybridCodeMap](HybridCodeMap.md) (OneOrMany) - Association to the set of HybridCodeMaps in the HybridCodelistMap.

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description




