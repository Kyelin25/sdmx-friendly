
# Organisation

Inherits from: [Item](../Base/Item.md)

## Subclasses

[Agency](Agency.md)

[DataProvider](DataProvider.md)

[DataConsumer](DataConsumer.md)

[OrganisationUnit](OrganisationUnit.md)



An organisation is a unique framework of authority within which a person or persons act, or are designated to act, towards some purpose.

## Attributes

id: string

uri: Url

urn: Urn



## References

contact: [Contact](Contact.md) (One) - Association to the Contact information.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

child: [Item](../Base/Item.md) (ZeroOrMany) - A child of this item.



## Referenced By

[ItemScheme](../Base/ItemScheme.md) (as items)

[ItemAssociation](../ItemSchemeMaps/ItemAssociation.md) (as source)

[ItemAssociation](../ItemSchemeMaps/ItemAssociation.md) (as target)


