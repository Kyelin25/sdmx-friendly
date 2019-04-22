
# StructureSet

Inherits from: [MaintainableArtefact](../Base/MaintainableArtefact.md)



A maintainable collection of structural maps that link components together in a source/target relationship where this is a semantic equivalence between the source and target Components.

## Attributes

id: string

uri: Url

urn: Urn

version: A version string following an agreed convention.

validFrom: Date from which the version is valid.

validTo: Date from which version is superceded.

final: Defines whether a maintained artefact is draft or final.

isExternalReference: If set to "true" it indicates that the content of the object is held externally. 

serviceUrl: The URL of an SDMX-compliant web service from which the external object can be retrieved.

structureUrl: The URL of an SDMX-ML document containing the external object



## References

relatedStructure: [Structure](../Base/Structure.md) (ZeroOrMany) - Association to a set of DataStructureDefinitions and MetadataStructureDefinitions.

relatedStructureUsage: [StructureUsage](../Base/StructureUsage.md) (ZeroOrMany) - Association to a set of DataflowDefinitions and MetadataflowDefinitions.

map: [StructureMap](StructureMap.md) (ZeroOrMany) - Association to StructureMaps.

itemSchemeMap: [ItemSchemeMap](../ItemSchemeMaps/ItemSchemeMap.md) (ZeroOrMany) - Association to a ItemSchemeMaps.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description



