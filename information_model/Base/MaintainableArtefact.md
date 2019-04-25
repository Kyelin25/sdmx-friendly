
# MaintainableArtefact

Inherits from: [VersionableArtefact](VersionableArtefact.md)

## Subclasses

[ItemScheme](ItemScheme.md)

[Structure](Structure.md)

[StructureUsage](StructureUsage.md)

[HierarchicalCodelist](../HierarchicalCodelists/HierarchicalCodelist.md)

[StructureSet](../StructureMaps/StructureSet.md)

[Constraint](../Constraints/Constraint.md)

[Process](../Process/Process.md)



## Description

An abstract class to group together primary structural metadata artefacts that are maintained by an Agency.


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

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description

name: [InternationalString](InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](Annotation.md) (ZeroOrMany) - No description




