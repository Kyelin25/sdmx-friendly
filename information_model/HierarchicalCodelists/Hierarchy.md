
# Hierarchy

Inherits from: [NameableArtefact](../Base/NameableArtefact.md)



## Description

A classification structure arranged in levels of detail from the broadest to the most detailed level.


## Attributes

**hasFormalLevels** (*bool*): If "true" this indicates a hierarchy where the structure is arranged in the levels of detail from the broadest to the most detailed level. If "false" this indicates a hierarchy structure where the items in the hierarchy have no formal level structure.

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

codes: [HierarchicalCode](HierarchicalCode.md) (ZeroOrMany) - Association to the top-level HierarchicalCodes in the Hierarchy.

level: [Level](Level.md) (ZeroOrOne) - Association to the top Level in the Hierarchy.

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[HierarchicalCodelist](HierarchicalCodelist.md) (as hierarchy)

[HierarchicalCodeReference](../HybridCodelistMap/HierarchicalCodeReference.md) (as hierarchy)


