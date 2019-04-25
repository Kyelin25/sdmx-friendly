
# Structure

Inherits from: [MaintainableArtefact](MaintainableArtefact.md)

## Subclasses

[DataStructureDefinition](../DataStructureDefinitions/DataStructureDefinition.md)

[MetadataStructureDefinition](../MetadataStructureDefinitions/MetadataStructureDefinition.md)



## Description

Abstract specification of a list of lists to define a complex tabular structure. A concrete example of this would be statistical Concepts, Codelists, and their organisation in a DataStructureDefinition or MetadataStructureDefinition, defined by a central institution, usually for the exchange of statistical information with its partners.


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

grouping: [ComponentList](ComponentList.md) (OneOrMany) - A composite association to one or more ComponentLists.

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description

name: [InternationalString](InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](Annotation.md) (ZeroOrMany) - No description



## Referenced By

[StructureUsage](StructureUsage.md) (as structure)

[StructureSet](../StructureMaps/StructureSet.md) (as relatedStructure)

[ReportingCategory](../ReportingTaxonomies/ReportingCategory.md) (as structure)


