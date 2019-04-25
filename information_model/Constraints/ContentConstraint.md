
# ContentConstraint

Inherits from: [Constraint](Constraint.md)



## Description

Defines a Constraint in terms of the content that can be found in data or metadata sources linked to the ConstrainableArtefact to which this constraint is associated.


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

dataContentRegion: [CubeRegion](CubeRegion.md) (ZeroOrMany) - Association to a subset of Component values that can be derived from the DataStructureDefinition to which the ConstrainableArtefact is linked.

metadataContentRegion: [MetadataTargetRegion](MetadataTargetRegion.md) (ZeroOrMany) - Association to a subset of Component values that can be derived from the MetadataStructureDefinition to which the ConstrainableArtefact is linked.

availableDates: [ReferencePeriod](ReferencePeriod.md) (ZeroOrOne) - Association to the time period that identifies the time range for which data or metadata are available in the data source.

contains: [ReleaseCalendar](ReleaseCalendar.md) (ZeroOrOne) - Association to a ReleaseCalendar

dataContentKeys: [DataKeySet](DataKeySet.md) (ZeroOrMany) - Association to a subset of DataKeySets (i.e. value combinations) that can be derived from the definition of the structure to which the ConstrainableArtefact is linked.

metadataContentKeys: [MetadataKeySet](MetadataKeySet.md) (ZeroOrMany) - Association to a subset of MetadataKeySets (i.e. value combinations) that can be derived from the definition of the Structure to which the ConstrainableArtefact is linked.

role: [ConstraintRole](ConstraintRole.md) (OneOrMany) - Association to the role that the Constraint plays.

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.



## Referenced By

[ConstrainableArtefact](ConstrainableArtefact.md) (as content)

[DataStructureDefinition](../DataStructureDefinitions/DataStructureDefinition.md) (as content)

[MetadataStructureDefinition](../MetadataStructureDefinitions/MetadataStructureDefinition.md) (as content)

[DataflowDefinition](../DataStructureDefinitions/DataflowDefinition.md) (as content)

[MetadataFlowDefinition](../MetadataStructureDefinitions/MetadataFlowDefinition.md) (as content)

[DataProvider](../OrganisationSchemes/DataProvider.md) (as content)

[DataSet](../DataStructureDefinitions/DataSet.md) (as content)

[GenericDataSet](../DataStructureDefinitions/GenericDataSet.md) (as content)

[StructureSpecificDataSet](../DataStructureDefinitions/StructureSpecificDataSet.md) (as content)

[GenericTimeseriesDataSet](../DataStructureDefinitions/GenericTimeseriesDataSet.md) (as content)

[StructureSpecificTimeseriesDataSet](../DataStructureDefinitions/StructureSpecificTimeseriesDataSet.md) (as content)

[ProvisionAgreement](../DataProvisioning/ProvisionAgreement.md) (as content)

[SimpleDatasource](../DataProvisioning/SimpleDatasource.md) (as content)

[WebServicesDatasource](../DataProvisioning/WebServicesDatasource.md) (as content)

[RESTDatasource](../DataProvisioning/RESTDatasource.md) (as content)

[SOAPDatasource](../DataProvisioning/SOAPDatasource.md) (as content)


