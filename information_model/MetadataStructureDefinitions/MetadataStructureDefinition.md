
# MetadataStructureDefinition

Inherits from: [Structure](../Base/Structure.md)



A collection of metadata concepts, their structure and usage when used to collect or disseminate reference metadata.

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

grouping: [MetadataTarget](MetadataTarget.md) (OneOrMany) - An association to a MetadataTarget or ReportStructure.

grouping: [ReportStructure](ReportStructure.md) (OneOrMany) - An association to a MetadataTarget or ReportStructure.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description



## Referenced By

[MetadataSet](MetadataSet.md) (as structuredBy)


