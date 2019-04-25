
# StructureSet

Inherits from: [MaintainableArtefact](../Base/MaintainableArtefact.md)



## Description

A maintainable collection of structural maps that link components together in a source/target relationship where this is a semantic equivalence between the source and target Components.


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

relatedStructure: [Structure](../Base/Structure.md) (ZeroOrMany) - Association to a set of DataStructureDefinitions and MetadataStructureDefinitions.

relatedStructureUsage: [StructureUsage](../Base/StructureUsage.md) (ZeroOrMany) - Association to a set of DataflowDefinitions and MetadataflowDefinitions.

map: [StructureMap](StructureMap.md) (ZeroOrMany) - Association to StructureMaps.

itemSchemeMap: [ItemSchemeMap](../ItemSchemeMaps/ItemSchemeMap.md) (ZeroOrMany) - Association to a ItemSchemeMaps.

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description




