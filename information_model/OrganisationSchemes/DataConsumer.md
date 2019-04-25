
# DataConsumer

Inherits from: [Organisation](Organisation.md)



## Description

An organisation using data as input for further processing.


## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.

### Inherited



## References

### Inherited

**contact** ([Contact](Contact.md) - 1): Association to the Contact information.
**child** ([DataConsumer](DataConsumer.md) - 0..*): A child of this DataConsumer
**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.
**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.
**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description


## Referenced By

[DataConsumerScheme](DataConsumerScheme.md) (as items)

[DataConsumer](DataConsumer.md) (as child)


