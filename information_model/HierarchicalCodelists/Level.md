
# Level

Inherits from: [NameableArtefact](../Base/NameableArtefact.md)



## Description

In a "level based" hierarchy this describes a group of Codes which are characterised by homogeneous coding, and where the parent of each Code in the group is at the same higher level of the Hierarchy. In a "value based" hierarchy this describes information about the HierarchicalCodes at the specified nesting level.


## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

**codeFormat** ([CodingFormat](CodingFormat.md) - 0..*): Association to the CodingFormat.

**child** ([Level](Level.md) - 0..*): Association to a child Level of Level.

**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description



## Referenced By

[Level](Level.md) (as child)

[Hierarchy](Hierarchy.md) (as level)

[HierarchicalCode](HierarchicalCode.md) (as level)


