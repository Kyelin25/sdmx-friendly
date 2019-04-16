
# Item

Inherits from: [NameableArtefact](NameableArtefact.md)

## Subclasses

[Code](../Codelists/Code.md)



The Item is an item of content in an ItemScheme. This may be a node in a taxonomy or ontology, a Code in a Codelist etc. Note that at the conceptual level the Organisation is not hierarchic.

## Attributes

id: string

uri: Url

urn: Urn



## References

child: [Item](Item.md) (ZeroOrMany) - A child of this item.

contains: [Annotation](Annotation.md) (ZeroOrMany) - No description

name: [InternationalString](InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.



## Referenced By

[ItemScheme](ItemScheme.md) (as items)

[Item](Item.md) (as child)

[Item](Item.md) (as child)


