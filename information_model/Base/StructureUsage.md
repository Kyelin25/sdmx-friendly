
# StructureUsage

Inherits from: [MaintainableArtefact](MaintainableArtefact.md)

## Subclasses

[DataflowDefinition](../DataStructureDefinitions/DataflowDefinition.md)

[MetadataFlowDefinition](../MetadataStructureDefinitions/MetadataFlowDefinition.md)



An artefact whose components are described by a Structure. In concrete terms (sub-classes) an example would be a DataflowDefinition which is linked to a given structure - in t his case the DataStructureDefinition.

## Attributes

id: string

uri: Url

urn: Urn

version: A version string following an agreed convention.

validFrom: Date from which the version is valid.

validTo: Date from which version is superceded.

final: Defines whether a maintained artefact is draft or final.

isExternalReference: If set to "true" it indicates that the content of the object is held externally. 

serviceUrl: The URL of an SDMX-compliant web service from which the external object can be retrieved.

structureUrl: The URL of an SDMX-ML document containing the external object



## References

structure: [Structure](Structure.md) (ZeroOrMany) - An association to a Structure specifying the structure of the artefact.

contains: [Annotation](Annotation.md) (ZeroOrMany) - No description

name: [InternationalString](InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description



## Referenced By

[StructureSet](../StructureMaps/StructureSet.md) (as relatedStructureUsage)

[ReportingCategory](../ReportingTaxonomies/ReportingCategory.md) (as flow)


