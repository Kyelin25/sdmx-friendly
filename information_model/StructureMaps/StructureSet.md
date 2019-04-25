
# StructureSet

Inherits from: [MaintainableArtefact](../Base/MaintainableArtefact.md)



## Description

A maintainable collection of structural maps that link components together in a source/target relationship where this is a semantic equivalence between the source and target Components.


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

**relatedStructure** ([Structure](../Base/Structure.md) - 0..*): Association to a set of DataStructureDefinitions and MetadataStructureDefinitions.

**relatedStructureUsage** ([StructureUsage](../Base/StructureUsage.md) - 0..*): Association to a set of DataflowDefinitions and MetadataflowDefinitions.

**map** ([StructureMap](StructureMap.md) - 0..*): Association to StructureMaps.

**itemSchemeMap** ([ItemSchemeMap](../ItemSchemeMaps/ItemSchemeMap.md) - 0..*): Association to a ItemSchemeMaps.

### Inherited

**maintainer** ([Agency](../OrganisationSchemes/Agency.md) - 1): No description

**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description




