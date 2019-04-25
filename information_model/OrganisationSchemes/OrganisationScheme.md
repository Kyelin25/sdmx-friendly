
# OrganisationScheme

Inherits from: [ItemScheme](../Base/ItemScheme.md)

## Subclasses

[AgencyScheme](AgencyScheme.md)

[DataProviderScheme](DataProviderScheme.md)

[DataConsumerScheme](DataConsumerScheme.md)

[OrganisationUnitScheme](OrganisationUnitScheme.md)



## Description

A maintained collection of Organisations.


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

items: [Organisation](Organisation.md) (ZeroOrMany) - Association to the Organisations in the OrganisationScheme.

maintainer: [Agency](Agency.md) (One) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[OrganisationSchemeMap](../ItemSchemeMaps/OrganisationSchemeMap.md) (as source)

[OrganisationSchemeMap](../ItemSchemeMaps/OrganisationSchemeMap.md) (as target)


