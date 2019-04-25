
# DataConsumer

Inherits from: [Organisation](Organisation.md)



## Description

An organisation using data as input for further processing.


## Attributes

id: string

uri: Url

urn: Urn



## References

contact: [Contact](Contact.md) (One) - Association to the Contact information.

child: [DataConsumer](DataConsumer.md) (ZeroOrMany) - A child of this DataConsumer

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[DataConsumerScheme](DataConsumerScheme.md) (as items)

[DataConsumer](DataConsumer.md) (as child)


