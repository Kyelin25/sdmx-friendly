
# StructureMap

Inherits from: [NameableArtefact](../Base/NameableArtefact.md)



## Description

Links a source and target structure where there is a semantic equivalence between the source and the target structures.


## Attributes

isExtension: bool

alias: string

id: string

uri: Url

urn: Urn



## References

map: [ComponentMap](ComponentMap.md) (OneOrMany) - Association to the ComponentMap.

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[StructureSet](StructureSet.md) (as map)


