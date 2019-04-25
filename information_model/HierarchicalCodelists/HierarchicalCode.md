
# HierarchicalCode

Inherits from: [IdentifiableArtefact](../Base/IdentifiableArtefact.md)



## Description

A hierarchic structure of code references.


## Attributes

**validFrom** (*Date*): Date from which construct is valid.

**validTo** (*Date*): Date from which construct is superceded.

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

code: [Code](../Codelists/Code.md) (One) - Association to the Code that is used at the specific point in the hierarchy.

child: [HierarchicalCode](HierarchicalCode.md) (ZeroOrMany) - Association to a child Code in the hierarchy.

level: [Level](Level.md) (ZeroOrOne) - Association to a Level where levels have been defined for the Hierarchy.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[Hierarchy](Hierarchy.md) (as codes)

[HierarchicalCode](HierarchicalCode.md) (as child)

[HierarchicalCodeReference](../HybridCodelistMap/HierarchicalCodeReference.md) (as codeAssociation)


