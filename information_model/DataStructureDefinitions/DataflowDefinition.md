
# DataflowDefinition

Inherits from: [StructureUsage](../Base/StructureUsage.md), [ConstrainableArtefact](../Constraints/ConstrainableArtefact.md)



## Description

Abstract concept (i.e. the structure without any data) of a flow of data that providers will provide for difference reference periods.


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

structure: [DataStructureDefinition](DataStructureDefinition.md) (ZeroOrMany) - Associates a DataflowDefinition to the DataStructureDefinition.

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

content: [ContentConstraint](../Constraints/ContentConstraint.md) (ZeroOrMany) - Associates the metadata that constrains the content to be found in a data or metadata source linked to the ConstrainableArtefact.

attachment: [AttachmentConstraint](../Constraints/AttachmentConstraint.md) (ZeroOrMany) - Associates the metadata that constrains the valid content of a ConstrainableArtefact to which metadata may be attached.



## Referenced By

[DataSet](DataSet.md) (as describedBy)

[GenericDataSet](GenericDataSet.md) (as describedBy)

[StructureSpecificDataSet](StructureSpecificDataSet.md) (as describedBy)

[GenericTimeseriesDataSet](GenericTimeseriesDataSet.md) (as describedBy)

[StructureSpecificTimeseriesDataSet](StructureSpecificTimeseriesDataSet.md) (as describedBy)


