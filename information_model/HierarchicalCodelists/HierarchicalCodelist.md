
# HierarchicalCodelist

Inherits from: [MaintainableArtefact](../Base/MaintainableArtefact.md)



## Description

An organised collection of codes that may participate in many parent/child relationships with other Codes in the scheme, as defined by one or more Hierarchy of the scheme.


## Attributes

final: bool

isExternalReference: bool

serviceUrl: Url

structureUrl: Url

version: string

validFrom: Date

validTo: Date

id: string

uri: Url

urn: Urn



## References

hierarchy: [Hierarchy](Hierarchy.md) (OneOrMany) - Association to Hierarchies of Codes

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[SourceHierarchicalCodelist](../HybridCodelistMap/SourceHierarchicalCodelist.md) (as hierarchicalCodelist)

[TargetHierarchicalCodelist](../HybridCodelistMap/TargetHierarchicalCodelist.md) (as hierarchicalCodelist)


