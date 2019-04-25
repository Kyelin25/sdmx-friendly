
# Code

Inherits from: [Item](../Base/Item.md)



## Description

A language independent set of letters, numbers of symbols that represent a concept whose meaning is described in a natural language.


## Attributes

id: string

uri: Url

urn: Urn



## References

child: [Code](Code.md) (ZeroOrMany) - A child of this Code

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[Codelist](Codelist.md) (as items)

[Code](Code.md) (as child)

[HierarchicalCode](../HierarchicalCodelists/HierarchicalCode.md) (as code)

[CodeMap](../ItemSchemeMaps/CodeMap.md) (as source)

[CodeMap](../ItemSchemeMaps/CodeMap.md) (as target)

[CodedAttributeValue](../DataStructureDefinitions/CodedAttributeValue.md) (as value)

[CodedKeyValue](../DataStructureDefinitions/CodedKeyValue.md) (as value)

[CodedObservation](../DataStructureDefinitions/CodedObservation.md) (as value)

[EnumeratedAttributeValue](../MetadataStructureDefinitions/EnumeratedAttributeValue.md) (as value)

[SourceCode](../HybridCodelistMap/SourceCode.md) (as code)

[TargetCode](../HybridCodelistMap/TargetCode.md) (as code)


