
# Level

Inherits from: [NameableArtefact](../Base/NameableArtefact.md)



In a "level based" hierarchy this describes a group of Codes which are characterised by homogeneous coding, and where the parent of each Code in the group is at the same higher level of the Hierarchy. In a "value based" hierarchy this describes information about the HierarchicalCodes at the specified nesting level.

## Attributes

id: string

uri: Url

urn: Urn



## References

codeFormat: [CodingFormat](CodingFormat.md) (ZeroOrMany) - Association to the CodingFormat.

child: [Level](Level.md) (ZeroOrMany) - Association to a child Level of Level.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.



## Referenced By

[Level](Level.md) (as child)

[Hierarchy](Hierarchy.md) (as level)

[HierarchicalCode](HierarchicalCode.md) (as level)

