
# CategoryScheme

Inherits from: [ItemScheme](../Base/ItemScheme.md)



## Description

The descriptive information for an arrangement or division of categories into groups based on characteristics, which the objects have in common.


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

items: [Category](Category.md) (ZeroOrMany) - Association to the Categories in the CategoryScheme.

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[CategorySchemeMap](../ItemSchemeMaps/CategorySchemeMap.md) (as source)

[CategorySchemeMap](../ItemSchemeMaps/CategorySchemeMap.md) (as target)


