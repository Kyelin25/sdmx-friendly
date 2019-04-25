
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

final: Defines whether a maintained artefact is draft or final.

isExternalReference: If set to "true" it indicates that the content of the object is held externally. 

serviceUrl: The URL of an SDMX-compliant web service from which the external object can be retrieved.

structureUrl: The URL of an SDMX-ML document containing the external object

version: A version string following an agreed convention.

validFrom: Date from which the version is valid.

validTo: Date from which version is superceded.

id: string

uri: Url

urn: Urn



## References

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description

name: [InternationalString](InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](Annotation.md) (ZeroOrMany) - No description




