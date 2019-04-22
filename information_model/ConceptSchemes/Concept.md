
# Concept

Inherits from: [Item](../Base/Item.md)



A concept is a unit of knowledge created by a unique combination of characteristics.

## Attributes

id: string

uri: Url

urn: Urn



## References

coreRepresentation: [Representation](../Base/Representation.md) (ZeroOrOne) - Associates a Representation.

ISOConcept: [ISOConcept](ISOConcept.md) (ZeroOrOne) - Association to an ISO concept reference.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

child: [Item](../Base/Item.md) (ZeroOrMany) - A child of this item.



## Referenced By

[ItemScheme](../Base/ItemScheme.md) (as items)

[Component](../Base/Component.md) (as conceptIdentity)

[Dimension](../DataStructureDefinitions/Dimension.md) (as role)

[Component](../Base/Component.md) (as conceptIdentity)

[Component](../Base/Component.md) (as conceptIdentity)

[Dimension](../DataStructureDefinitions/Dimension.md) (as role)

[Component](../Base/Component.md) (as conceptIdentity)

[Dimension](../DataStructureDefinitions/Dimension.md) (as role)

[DataAttribute](../DataStructureDefinitions/DataAttribute.md) (as role)

[Component](../Base/Component.md) (as conceptIdentity)

[Component](../Base/Component.md) (as conceptIdentity)

[DataAttribute](../DataStructureDefinitions/DataAttribute.md) (as role)

[Component](../Base/Component.md) (as conceptIdentity)

[Component](../Base/Component.md) (as conceptIdentity)

[Component](../Base/Component.md) (as conceptIdentity)

[Component](../Base/Component.md) (as conceptIdentity)

[Component](../Base/Component.md) (as conceptIdentity)

[Component](../Base/Component.md) (as conceptIdentity)

[Component](../Base/Component.md) (as conceptIdentity)

[Component](../Base/Component.md) (as conceptIdentity)

[ItemAssociation](../ItemSchemeMaps/ItemAssociation.md) (as source)

[ItemAssociation](../ItemSchemeMaps/ItemAssociation.md) (as target)

[MeasureKeyValue](../DataStructureDefinitions/MeasureKeyValue.md) (as value)

[ConceptUsage](../MetadataStructureDefinitions/ConceptUsage.md) (as concept)


