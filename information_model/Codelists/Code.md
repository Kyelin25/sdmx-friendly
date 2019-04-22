
# Code

Inherits from: [Item](../Base/Item.md)



A language independent set of letters, numbers of symbols that represent a concept whose meaning is described in a natural language.

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

[HierarchicalCode](../HierarchicalCodelists/HierarchicalCode.md) (as code)

[ItemAssociation](../ItemSchemeMaps/ItemAssociation.md) (as source)

[ItemAssociation](../ItemSchemeMaps/ItemAssociation.md) (as target)

[CodedAttributeValue](../DataStructureDefinitions/CodedAttributeValue.md) (as value)

[CodedKeyValue](../DataStructureDefinitions/CodedKeyValue.md) (as value)

[CodedObservation](../DataStructureDefinitions/CodedObservation.md) (as value)

[EnumeratedAttributeValue](../MetadataStructureDefinitions/EnumeratedAttributeValue.md) (as value)

[SourceCode](../HybridCodelistMap/SourceCode.md) (as code)

[TargetCode](../HybridCodelistMap/TargetCode.md) (as code)


