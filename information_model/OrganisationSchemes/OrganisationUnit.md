
# OrganisationUnit

Inherits from: [Organisation](Organisation.md)



A designation in the organisational structure.

## Attributes

id: string

uri: Url

urn: Urn



## References

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

child: [Item](../Base/Item.md) (ZeroOrMany) - A child of this item.

contact: [Contact](Contact.md) (One) - Association to the Contact information.



## Referenced By

[ItemScheme](../Base/ItemScheme.md) (as items)


