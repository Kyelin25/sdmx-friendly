
# Category

Inherits from: [Item](../Base/Item.md)



## Description

An item at any level within a classification, typically tabulation categories, sections, subsections, divisions, subdivisions, groups, subgroups, classes and subclasses.


## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.

### Inherited



## References

**child** ([Category](Category.md) - 0..*): A child of this Category

**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description

### Inherited



## Referenced By

[CategoryScheme](CategoryScheme.md) (as items)

[Category](Category.md) (as child)

[CategoryMap](../ItemSchemeMaps/CategoryMap.md) (as source)

[CategoryMap](../ItemSchemeMaps/CategoryMap.md) (as target)

[Categorisation](Categorisation.md) (as categorisedBy)


