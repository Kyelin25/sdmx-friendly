
# StructureSpecificDataSet

Inherits from: [DataSet](DataSet.md)



## Description

A data format structure that contains data corresponding to one specific DataStructureDefinition.


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



## References

describedBy: [DataflowDefinition](DataflowDefinition.md) (ZeroOrOne) - Associates a DataflowDefinition and thereby a DataStructureDefinition to the DataSet.

structuredBy: [DataStructureDefinition](DataStructureDefinition.md) (One) - Associates the DataStructureDefinition that defines the structure of the DataSet. Note that the DataStructureDefinition is the same as that associated (non-mandatory) to the DataflowDefinition.

publishedBy: [DataProvider](../OrganisationSchemes/DataProvider.md) (ZeroOrOne) - Association to the DataProvider that reports/publishes the data.

attachedAttribute: [AttributeValue](AttributeValue.md) (ZeroOrMany) - Association to the AttributeValues relating to the DataSet.

content: [ContentConstraint](../Constraints/ContentConstraint.md) (ZeroOrMany) - Associates the metadata that constrains the content to be found in a data or metadata source linked to the ConstrainableArtefact.

attachment: [AttachmentConstraint](../Constraints/AttachmentConstraint.md) (ZeroOrMany) - Associates the metadata that constrains the valid content of a ConstrainableArtefact to which metadata may be attached.




