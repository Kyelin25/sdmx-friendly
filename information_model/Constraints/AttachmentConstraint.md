
# AttachmentConstraint

Inherits from: [Constraint](Constraint.md)



## Description

Defines a Constraint in terms of the combination of Component values that may be found in a data source, and to which a ConstrainableArtefact may be associated in a structure definition.


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

**dataContentKeys** ([DataKeySet](DataKeySet.md) - 0..*): Association to a subset of DataKeySets (i.e. value combinations) that can be derived from the definition of the structure to which the ConstrainableArtefact is linked.
**metadataContentKeys** ([MetadataKeySet](MetadataKeySet.md) - 0..*): Association to a subset of MetadataKeySets (i.e. value combinations) that can be derived from the definition of the Structure to which the ConstrainableArtefact is linked.
**role** ([ConstraintRole](ConstraintRole.md) - 1..*): Association to the role that the Constraint plays.
**maintainer** ([Agency](../OrganisationSchemes/Agency.md) - 1): No description
**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.
**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.
**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description


## Referenced By

[ConstrainableArtefact](ConstrainableArtefact.md) (as attachment)

[DataStructureDefinition](../DataStructureDefinitions/DataStructureDefinition.md) (as attachment)

[MetadataStructureDefinition](../MetadataStructureDefinitions/MetadataStructureDefinition.md) (as attachment)

[DataflowDefinition](../DataStructureDefinitions/DataflowDefinition.md) (as attachment)

[MetadataFlowDefinition](../MetadataStructureDefinitions/MetadataFlowDefinition.md) (as attachment)

[DataProvider](../OrganisationSchemes/DataProvider.md) (as attachment)

[DataSet](../DataStructureDefinitions/DataSet.md) (as attachment)

[GenericDataSet](../DataStructureDefinitions/GenericDataSet.md) (as attachment)

[StructureSpecificDataSet](../DataStructureDefinitions/StructureSpecificDataSet.md) (as attachment)

[GenericTimeseriesDataSet](../DataStructureDefinitions/GenericTimeseriesDataSet.md) (as attachment)

[StructureSpecificTimeseriesDataSet](../DataStructureDefinitions/StructureSpecificTimeseriesDataSet.md) (as attachment)

[ProvisionAgreement](../DataProvisioning/ProvisionAgreement.md) (as attachment)

[SimpleDatasource](../DataProvisioning/SimpleDatasource.md) (as attachment)

[WebServicesDatasource](../DataProvisioning/WebServicesDatasource.md) (as attachment)

[RESTDatasource](../DataProvisioning/RESTDatasource.md) (as attachment)

[SOAPDatasource](../DataProvisioning/SOAPDatasource.md) (as attachment)


