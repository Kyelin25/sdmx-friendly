
# HybridCodelistMap

Inherits from: [NameableArtefact](../Base/NameableArtefact.md)



Associates a Codelist and a HierarchicalCodelist.

## Attributes

alias: string

id: string

uri: Url

urn: Urn



## References

source: [SourceList](SourceList.md) (One) - Association to the source List.

target: [TargetList](TargetList.md) (One) - Associationg to the target List.

hybridCodeMap: [HybridCodeMap](HybridCodeMap.md) (OneOrMany) - Association to the set of HybridCodeMaps in the HybridCodelistMap.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.




