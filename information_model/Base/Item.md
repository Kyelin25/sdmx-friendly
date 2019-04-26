
# Item

Inherits from: [NameableArtefact](NameableArtefact.md)

## Subclasses

[Code](../Codelist/Code.md)

[Concept](../ConceptScheme/Concept.md)

[Category](../CategoryScheme/Category.md)

[Organisation](Organisation.md)

[ReportingCategory](../CategoryScheme/ReportingCategory.md)



## Description

The Item is an item of content in an ItemScheme. This may be a node in a taxonomy or ontology, a Code in a Codelist etc. Note that at the conceptual level the Organisation is not hierarchic.


## Attributes

### Inherited

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

**child** ([Item](Item.md) - 0..*): A child of this item.

### Inherited

**name** ([InternationalString](InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

**contains** ([Annotation](Annotation.md) - 0..*): No description



## Referenced By

[ItemScheme](ItemScheme.md) (as items)

[Item](Item.md) (as child)

[ItemAssociation](../Mapping/ItemAssociation.md) (as source)

[ItemAssociation](../Mapping/ItemAssociation.md) (as target)


