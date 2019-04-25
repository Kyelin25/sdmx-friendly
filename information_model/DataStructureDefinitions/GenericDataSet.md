
# GenericDataSet

Inherits from: [DataSet](DataSet.md)



## Description

A data format structure that is able to contain data corresponding to any DataStructureDefinition.


## Attributes

**reportingBegin** (*Date*): A specific time period in a known system of time periods that identifies the start period of a report.

**reportingEnd** (*Date*): A specific time period in a known system of time periods that identifies the end period of a report.

**dataExtractionDate** (*Date*): A specific time period that identifies the date and time that the data are extracted from a data source.

**validFrom** (*Date*): Indicates the inclusive start time indicating the validity of the information in the DataSet.

**validTo** (*Date*): Indicates the inclusive end time indicating the validity of the information in the DataSet.

**publicationYear** (*Date*): Specifies the year of publication of the data or metadata in terms of whatever provisioning agreements might be in force.

**publicationPeriod** (*Date*): Specifies the period of publication of the data or metadata in terms of whatever provisioning agreements might be in force.

**setId** (*string*): Provides an identification of the DataSet.

**action** (*ActionType*): Defines the action to be taken by the recipient system (update, append, delete).

### Inherited



## References

**describedBy** ([DataflowDefinition](DataflowDefinition.md) - 0..1): Associates a DataflowDefinition and thereby a DataStructureDefinition to the DataSet.

**structuredBy** ([DataStructureDefinition](DataStructureDefinition.md) - 1): Associates the DataStructureDefinition that defines the structure of the DataSet. Note that the DataStructureDefinition is the same as that associated (non-mandatory) to the DataflowDefinition.

**publishedBy** ([DataProvider](../OrganisationSchemes/DataProvider.md) - 0..1): Association to the DataProvider that reports/publishes the data.

**attachedAttribute** ([AttributeValue](AttributeValue.md) - 0..*): Association to the AttributeValues relating to the DataSet.

**content** ([ContentConstraint](../Constraints/ContentConstraint.md) - 0..*): Associates the metadata that constrains the content to be found in a data or metadata source linked to the ConstrainableArtefact.

**attachment** ([AttachmentConstraint](../Constraints/AttachmentConstraint.md) - 0..*): Associates the metadata that constrains the valid content of a ConstrainableArtefact to which metadata may be attached.

### Inherited




