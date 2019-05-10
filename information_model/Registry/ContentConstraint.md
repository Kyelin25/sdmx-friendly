
# ContentConstraint



Inherits from: [Constraint](Constraint.md)



## Description

Defines a Constraint in terms of the content that can be found in data or metadata sources linked to the ConstrainableArtefact to which this constraint is associated.


## Attributes

### Inherited

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



## References

**dataContentRegion** ([CubeRegion](CubeRegion.md) - 0..*): Association to a subset of Component values that can be derived from the DataStructureDefinition to which the ConstrainableArtefact is linked.

**metadataContentRegion** ([MetadataTargetRegion](MetadataTargetRegion.md) - 0..*): Association to a subset of Component values that can be derived from the MetadataStructureDefinition to which the ConstrainableArtefact is linked.

**availableDates** ([ReferencePeriod](ReferencePeriod.md) - 0..1): Association to the time period that identifies the time range for which data or metadata are available in the data source.

**contains** ([ReleaseCalendar](ReleaseCalendar.md) - 0..1): Association to a ReleaseCalendar

### Inherited

**dataContentKeys** ([DataKeySet](DataKeySet.md) - 0..*): Association to a subset of DataKeySets (i.e. value combinations) that can be derived from the definition of the structure to which the ConstrainableArtefact is linked.

**metadataContentKeys** ([MetadataKeySet](MetadataKeySet.md) - 0..*): Association to a subset of MetadataKeySets (i.e. value combinations) that can be derived from the definition of the Structure to which the ConstrainableArtefact is linked.

**role** ([ConstraintRole](ConstraintRole.md) - 1..*): Association to the role that the Constraint plays.

**maintainer** ([Agency](../Base/Agency.md) - 1): No description

**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.



## Referenced By

[ConstrainableArtefact](ConstrainableArtefact.md) (as content)

[DataStructureDefinition](../DataStructure/DataStructureDefinition.md) (as content)

[MetadataStructureDefinition](../MetadataStructure/MetadataStructureDefinition.md) (as content)

[DataflowDefinition](../DataStructure/DataflowDefinition.md) (as content)

[MetadataFlowDefinition](../MetadataStructure/MetadataFlowDefinition.md) (as content)

[DataProvider](../Base/DataProvider.md) (as content)

[DataSet](../DataStructure/DataSet.md) (as content)

[GenericDataSet](../DataStructure/GenericDataSet.md) (as content)

[StructureSpecificDataSet](../DataStructure/StructureSpecificDataSet.md) (as content)

[GenericTimeseriesDataSet](../DataStructure/GenericTimeseriesDataSet.md) (as content)

[StructureSpecificTimeseriesDataSet](../DataStructure/StructureSpecificTimeseriesDataSet.md) (as content)

[ProvisionAgreement](ProvisionAgreement.md) (as content)

[SimpleDatasource](SimpleDatasource.md) (as content)

[WebServicesDatasource](WebServicesDatasource.md) (as content)

[RESTDatasource](RESTDatasource.md) (as content)

[SOAPDatasource](SOAPDatasource.md) (as content)


