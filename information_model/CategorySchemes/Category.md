
# Category

Inherits from: [Item](../Base/Item.md)



An item at any level within a classification, typically tabulation categories, sections, subsections, divisions, subdivisions, groups, subgroups, classes and subclasses.

## Attributes

id: string

uri: Url

urn: Urn



## References

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

child: [Item](../Base/Item.md) (ZeroOrMany) - A child of this item.



## Referenced By

[ItemScheme](../Base/ItemScheme.md) (as items)

[ItemAssociation](../ItemSchemeMaps/ItemAssociation.md) (as source)

[ItemAssociation](../ItemSchemeMaps/ItemAssociation.md) (as target)

[Categorisation](Categorisation.md) (as categorisedBy)


