
# ContentConstraint

Inherits from: [Constraint](Constraint.md)



## Description

Defines a Constraint in terms of the content that can be found in data or metadata sources linked to the ConstrainableArtefact to which this constraint is associated.


## Attributes

**final** (*bool*): Defines whether a maintained artefact is draft or final.

**isExternalReference** (*bool*): If set to "true" it indicates that the content of the object is held externally.

**serviceUrl** (*Url*): The URL of an SDMX-compliant web service from which the external object can be retrieved.

**structureUrl** (*Url*): The URL of an SDMX-ML document containing the external object

**version** (*string*): A version string following an agreed convention.

**validFrom** (*Date*): Date from which the version is valid.

**validTo** (*Date*): Date from which version is superceded.

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.

### Inherited



## References

### Inherited

**dataContentRegion** ([CubeRegion](CubeRegion.md) - 0..*): Association to a subset of Component values that can be derived from the DataStructureDefinition to which the ConstrainableArtefact is linked.
**metadataContentRegion** ([MetadataTargetRegion](MetadataTargetRegion.md) - 0..*): Association to a subset of Component values that can be derived from the MetadataStructureDefinition to which the ConstrainableArtefact is linked.
**availableDates** ([ReferencePeriod](ReferencePeriod.md) - 0..1): Association to the time period that identifies the time range for which data or metadata are available in the data source.
**contains** ([ReleaseCalendar](ReleaseCalendar.md) - 0..1): Association to a ReleaseCalendar
**dataContentKeys** ([DataKeySet](DataKeySet.md) - 0..*): Association to a subset of DataKeySets (i.e. value combinations) that can be derived from the definition of the structure to which the ConstrainableArtefact is linked.
**metadataContentKeys** ([MetadataKeySet](MetadataKeySet.md) - 0..*): Association to a subset of MetadataKeySets (i.e. value combinations) that can be derived from the definition of the Structure to which the ConstrainableArtefact is linked.
**role** ([ConstraintRole](ConstraintRole.md) - 1..*): Association to the role that the Constraint plays.
**maintainer** ([Agency](../OrganisationSchemes/Agency.md) - 1): No description
**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.
**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.


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


