
# Item

Inherits from: [NameableArtefact](NameableArtefact.md)

## Subclasses

[Code](../Codelists/Code.md)

[Concept](../ConceptSchemes/Concept.md)

[Category](../CategorySchemes/Category.md)

[Organisation](../OrganisationSchemes/Organisation.md)

[ReportingCategory](../ReportingTaxonomies/ReportingCategory.md)



## Description

The Item is an item of content in an ItemScheme. This may be a node in a taxonomy or ontology, a Code in a Codelist etc. Note that at the conceptual level the Organisation is not hierarchic.


## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.

### Inherited



## References

### Inherited

**child** ([Item](Item.md) - 0..*): A child of this item.
**name** ([InternationalString](InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.
**description** ([InternationalString](InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.
**contains** ([Annotation](Annotation.md) - 0..*): No description


## Referenced By

[ItemScheme](ItemScheme.md) (as items)

[Item](Item.md) (as child)

[ItemAssociation](../ItemSchemeMaps/ItemAssociation.md) (as source)

[ItemAssociation](../ItemSchemeMaps/ItemAssociation.md) (as target)


