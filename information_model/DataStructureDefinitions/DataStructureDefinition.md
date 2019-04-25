
# DataStructureDefinition

Inherits from: [Structure](../Base/Structure.md), [ConstrainableArtefact](../Constraints/ConstrainableArtefact.md)



## Description

A collection of metadata concepts, their structure and usage when used to collect or disseminate data.


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

grouping: [ComponentList](../Base/ComponentList.md) (OneOrMany) - An association to a set of metadata concepts that have an identified structural role in a DataStructureDefinition.

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

content: [ContentConstraint](../Constraints/ContentConstraint.md) (ZeroOrMany) - Associates the metadata that constrains the content to be found in a data or metadata source linked to the ConstrainableArtefact.

attachment: [AttachmentConstraint](../Constraints/AttachmentConstraint.md) (ZeroOrMany) - Associates the metadata that constrains the valid content of a ConstrainableArtefact to which metadata may be attached.



## Referenced By

[DataflowDefinition](DataflowDefinition.md) (as structure)

[MetadataFlowDefinition](../MetadataStructureDefinitions/MetadataFlowDefinition.md) (as structure)

[DataSet](DataSet.md) (as structuredBy)

[GenericDataSet](GenericDataSet.md) (as structuredBy)

[StructureSpecificDataSet](StructureSpecificDataSet.md) (as structuredBy)

[GenericTimeseriesDataSet](GenericTimeseriesDataSet.md) (as structuredBy)

[StructureSpecificTimeseriesDataSet](StructureSpecificTimeseriesDataSet.md) (as structuredBy)


