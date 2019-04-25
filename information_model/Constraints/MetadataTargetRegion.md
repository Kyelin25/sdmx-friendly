
# MetadataTargetRegion





## Description

A set of Components and their values that defines a subset or "slice" of the total range of possible content of a MetadataStructureDefinition to which the ConstrainableArtefact is linked.


## Attributes

**isIncluded** (*bool*): Indicates whether the MetadataTargetRegion is included in the Constraint definition or excluded from the Constraint definition.



## References

**componentList** ([ComponentList](../Base/ComponentList.md) - 1): Reference to the ComponentList. May be only conceptual.

**member** ([MemberSelection](MemberSelection.md) - 0..*): Associates the set of Components that define the subset of values.



## Referenced By

[ContentConstraint](ContentConstraint.md) (as metadataContentRegion)


