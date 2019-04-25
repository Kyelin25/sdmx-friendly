
# StructureUsage

Inherits from: [MaintainableArtefact](MaintainableArtefact.md)

## Subclasses

[DataflowDefinition](../DataStructureDefinitions/DataflowDefinition.md)

[MetadataFlowDefinition](../MetadataStructureDefinitions/MetadataFlowDefinition.md)



## Description

An artefact whose components are described by a Structure. In concrete terms (sub-classes) an example would be a DataflowDefinition which is linked to a given structure - in t his case the DataStructureDefinition.


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

**structure** ([Structure](Structure.md) - 0..*): An association to a Structure specifying the structure of the artefact.

### Inherited

**maintainer** ([Agency](../OrganisationSchemes/Agency.md) - 1): No description

**name** ([InternationalString](InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

**contains** ([Annotation](Annotation.md) - 0..*): No description



## Referenced By

[StructureSet](../StructureMaps/StructureSet.md) (as relatedStructureUsage)

[ReportingCategory](../ReportingTaxonomies/ReportingCategory.md) (as flow)

[ProvisionAgreement](../DataProvisioning/ProvisionAgreement.md) (as controlledBy)


