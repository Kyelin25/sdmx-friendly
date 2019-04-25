
# DataStructureDefinition

Inherits from: [Structure](../Base/Structure.md), [ConstrainableArtefact](../Constraints/ConstrainableArtefact.md)



## Description

A collection of metadata concepts, their structure and usage when used to collect or disseminate data.


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

**grouping** ([ComponentList](../Base/ComponentList.md) - 1..*): An association to a set of metadata concepts that have an identified structural role in a DataStructureDefinition.
**maintainer** ([Agency](../OrganisationSchemes/Agency.md) - 1): No description
**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.
**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.
**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description
**content** ([ContentConstraint](../Constraints/ContentConstraint.md) - 0..*): Associates the metadata that constrains the content to be found in a data or metadata source linked to the ConstrainableArtefact.
**attachment** ([AttachmentConstraint](../Constraints/AttachmentConstraint.md) - 0..*): Associates the metadata that constrains the valid content of a ConstrainableArtefact to which metadata may be attached.


## Referenced By

[DataflowDefinition](DataflowDefinition.md) (as structure)

[MetadataFlowDefinition](../MetadataStructureDefinitions/MetadataFlowDefinition.md) (as structure)

[DataSet](DataSet.md) (as structuredBy)

[GenericDataSet](GenericDataSet.md) (as structuredBy)

[StructureSpecificDataSet](StructureSpecificDataSet.md) (as structuredBy)

[GenericTimeseriesDataSet](GenericTimeseriesDataSet.md) (as structuredBy)

[StructureSpecificTimeseriesDataSet](StructureSpecificTimeseriesDataSet.md) (as structuredBy)


