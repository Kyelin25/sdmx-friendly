
# Organisation

*Abstract*

Inherits from: [Item](Item.md)

## Subclasses

[Agency](Agency.md)

[DataProvider](DataProvider.md)

[DataConsumer](DataConsumer.md)

[OrganisationUnit](OrganisationUnit.md)



## Description

An organisation is a unique framework of authority within which a person or persons act, or are designated to act, towards some purpose.


## Attributes

### Inherited

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

**contact** ([Contact](Contact.md) - 1): Association to the Contact information.

### Inherited

**child** ([Organisation](Organisation.md) - 0..*): A child of this Organisation

**name** ([InternationalString](InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

**contains** ([Annotation](Annotation.md) - 0..*): No description



## Referenced By

[OrganisationScheme](OrganisationScheme.md) (as items)

[Organisation](Organisation.md) (as child)

[OrganisationMap](../Mapping/OrganisationMap.md) (as source)

[OrganisationMap](../Mapping/OrganisationMap.md) (as target)


