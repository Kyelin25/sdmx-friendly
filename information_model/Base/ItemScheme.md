
# ItemScheme

Inherits from: [MaintainableArtefact](MaintainableArtefact.md)

## Subclasses

[Codelist](../Codelists/Codelist.md)

[ConceptScheme](../ConceptSchemes/ConceptScheme.md)

[CategoryScheme](../CategorySchemes/CategoryScheme.md)

[OrganisationScheme](../OrganisationSchemes/OrganisationScheme.md)

[ReportingTaxonomy](../ReportingTaxonomies/ReportingTaxonomy.md)



## Description

The descriptive information for an arrangement or division of objects into groups based on characteristics, which the objects have in common.


## Attributes

isPartial: bool

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

items: [Item](Item.md) (ZeroOrMany) - Association to the Items in the scheme.

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description

name: [InternationalString](InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](Annotation.md) (ZeroOrMany) - No description



## Referenced By

[ItemSchemeMap](../ItemSchemeMaps/ItemSchemeMap.md) (as source)

[ItemSchemeMap](../ItemSchemeMaps/ItemSchemeMap.md) (as target)

[Representation](Representation.md) (as enumerated)


