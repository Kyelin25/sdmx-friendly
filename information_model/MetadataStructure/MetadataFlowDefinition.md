
# MetadataFlowDefinition



Inherits from: [StructureUsage](../Base/StructureUsage.md), [ConstrainableArtefact](../Registry/ConstrainableArtefact.md)



## Description

Abstract concept (i.e. the structure without any metadata) of a flow of metadata that providers will provide for difference reference periods.


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

### Inherited

**structure** ([DataStructureDefinition](../DataStructure/DataStructureDefinition.md) - 0..*): Associates a DataflowDefinition to the DataStructureDefinition.

**maintainer** ([Agency](../Base/Agency.md) - 1): No description

**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description

**content** ([ContentConstraint](../Registry/ContentConstraint.md) - 0..*): Associates the metadata that constrains the content to be found in a data or metadata source linked to the ConstrainableArtefact.

**attachment** ([AttachmentConstraint](../Registry/AttachmentConstraint.md) - 0..*): Associates the metadata that constrains the valid content of a ConstrainableArtefact to which metadata may be attached.



## Referenced By

[MetadataSet](MetadataSet.md) (as describedBy)


