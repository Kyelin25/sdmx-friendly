
# MetadataSet

Inherits from: [NameableArtefact](../Base/NameableArtefact.md)



Any organised collection of metadata.

## Attributes

reportingBegin: Date

reportingEnd: Date

dataExtractionDate: Date

validFrom: Date

validTo: Date

publicationYear: Date

publicationPeriod: Date

setId: string

action: ActionType

id: string

uri: Url

urn: Urn



## References

describedBy: [MetadataFlowDefinition](MetadataFlowDefinition.md) (ZeroOrOne) - Associates a MetadataflowDefinition to the MetadataSet.

structuredBy: [MetadataStructureDefinition](MetadataStructureDefinition.md) (One) - Associates the MetadataStructureDefinition that defines the structure of the MetadataSet. Note that the MetadataStructureDefinition is the same as that associated (non-mandatory) to the MetadataflowDefinition.

describedBy: [ReportStructure](ReportStructure.md) (One) - Reference to the ReportStructure.

publishedBy: [DataProvider](../OrganisationSchemes/DataProvider.md) (ZeroOrOne) - Assocates the DataProvider that reports/publishes the metadata.

contains: [MetadataReport](MetadataReport.md) (OneOrMany) - MetadataReports contained by this MetadataSet.

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.




