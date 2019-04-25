
# HierarchicalCode

Inherits from: [IdentifiableArtefact](../Base/IdentifiableArtefact.md)



## Description

A hierarchic structure of code references.


## Attributes

validFrom: Date

validTo: Date

id: string

uri: Url

urn: Urn



## References

code: [Code](../Codelists/Code.md) (One) - Association to the Code that is used at the specific point in the hierarchy.

child: [HierarchicalCode](HierarchicalCode.md) (ZeroOrMany) - Association to a child Code in the hierarchy.

level: [Level](Level.md) (ZeroOrOne) - Association to a Level where levels have been defined for the Hierarchy.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[Hierarchy](Hierarchy.md) (as codes)

[HierarchicalCode](HierarchicalCode.md) (as child)

[HierarchicalCodeReference](../HybridCodelistMap/HierarchicalCodeReference.md) (as codeAssociation)


