
# Hierarchy

Inherits from: [NameableArtefact](../Base/NameableArtefact.md)



A classification structure arranged in levels of detail from the broadest to the most detailed level.

## Attributes

hasFormalLevels: bool

id: string

uri: Url

urn: Urn



## References

codes: [HierarchicalCode](HierarchicalCode.md) (ZeroOrMany) - Association to the top-level HierarchicalCodes in the Hierarchy.

level: [Level](Level.md) (ZeroOrOne) - Association to the top Level in the Hierarchy.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.



## Referenced By

[HierarchicalCodelist](HierarchicalCodelist.md) (as hierarchy)

[HierarchicalCodeReference](../HybridCodelistMap/HierarchicalCodeReference.md) (as hierarchy)


