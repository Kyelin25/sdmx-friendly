
# StructureUsage

Inherits from: [MaintainableArtefact](MaintainableArtefact.md)

## Subclasses

[DataflowDefinition](../DataStructureDefinitions/DataflowDefinition.md)

[MetadataFlowDefinition](../MetadataStructureDefinitions/MetadataFlowDefinition.md)



## Description

An artefact whose components are described by a Structure. In concrete terms (sub-classes) an example would be a DataflowDefinition which is linked to a given structure - in t his case the DataStructureDefinition.


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

structure: [Structure](Structure.md) (ZeroOrMany) - An association to a Structure specifying the structure of the artefact.

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description

name: [InternationalString](InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](Annotation.md) (ZeroOrMany) - No description



## Referenced By

[StructureSet](../StructureMaps/StructureSet.md) (as relatedStructureUsage)

[ReportingCategory](../ReportingTaxonomies/ReportingCategory.md) (as flow)

[ProvisionAgreement](../DataProvisioning/ProvisionAgreement.md) (as controlledBy)


