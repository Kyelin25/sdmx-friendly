
# OrganisationUnit

Inherits from: [Organisation](Organisation.md)



## Description

A designation in the organisational structure.


## Attributes

id: string

uri: Url

urn: Urn



## References

contact: [Contact](Contact.md) (One) - Association to the Contact information.

child: [OrganisationUnit](OrganisationUnit.md) (ZeroOrMany) - A child of this OrganisationUnit

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[OrganisationUnitScheme](OrganisationUnitScheme.md) (as items)

[OrganisationUnit](OrganisationUnit.md) (as child)


