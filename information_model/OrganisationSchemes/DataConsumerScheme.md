
# DataConsumerScheme

Inherits from: [OrganisationScheme](OrganisationScheme.md)



## Description

A maintained collection of DataConsumers.


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

items: [DataConsumer](DataConsumer.md) (ZeroOrMany) - Association to the DataConsumers in the DataConsumerScheme.

maintainer: [Agency](Agency.md) (One) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description




