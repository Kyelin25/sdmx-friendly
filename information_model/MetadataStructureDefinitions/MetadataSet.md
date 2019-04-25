
# MetadataSet

Inherits from: [NameableArtefact](../Base/NameableArtefact.md)



## Description

Any organised collection of metadata.


## Attributes

**reportingBegin** (*Date*): A specific time period in a known system of time periods that identifies the start period of a report.

**reportingEnd** (*Date*): A specific time period in a known system of time periods that identifies the end period of a report.

**dataExtractionDate** (*Date*): A specific time period that identifies the date and time that the metadata are extracted from a metadata source.

**validFrom** (*Date*): Indicates the inclusive start time indicating the validity of the information in the MetadataSet.

**validTo** (*Date*): Indicates the inclusive end t ime indicating the validity of the information in the MetadataSet.

**publicationYear** (*Date*): Specifies the year of publication of the data or metadata in terms of whatever provisioning agreements might be in force.

**publicationPeriod** (*Date*): Specifies the period of publication of the data or metdata in terms of whatever provisioning agreements might be in force.

**setId** (*string*): Provides an identification of the MetadataSet.

**action** (*ActionType*): Defines the action to be taken by the recipient system (update, replace, delete).

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.

### Inherited



## References

### Inherited

**describedBy** ([MetadataFlowDefinition](MetadataFlowDefinition.md) - 0..1): Associates a MetadataflowDefinition to the MetadataSet.
**structuredBy** ([MetadataStructureDefinition](MetadataStructureDefinition.md) - 1): Associates the MetadataStructureDefinition that defines the structure of the MetadataSet. Note that the MetadataStructureDefinition is the same as that associated (non-mandatory) to the MetadataflowDefinition.
**describedBy** ([ReportStructure](ReportStructure.md) - 1): Reference to the ReportStructure.
**publishedBy** ([DataProvider](../OrganisationSchemes/DataProvider.md) - 0..1): Assocates the DataProvider that reports/publishes the metadata.
**contains** ([MetadataReport](MetadataReport.md) - 1..*): MetadataReports contained by this MetadataSet.
**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.
**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.



