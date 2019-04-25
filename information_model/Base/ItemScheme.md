
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

final: Defines whether a maintained artefact is draft or final.

isExternalReference: If set to "true" it indicates that the content of the object is held externally. 

serviceUrl: The URL of an SDMX-compliant web service from which the external object can be retrieved.

structureUrl: The URL of an SDMX-ML document containing the external object

version: A version string following an agreed convention.

validFrom: Date from which the version is valid.

validTo: Date from which version is superceded.

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


