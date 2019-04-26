
# Code

Inherits from: [Item](../Base/Item.md)



## Description

A language independent set of letters, numbers of symbols that represent a concept whose meaning is described in a natural language.


## Attributes

### Inherited

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

### Inherited

**child** ([Code](Code.md) - 0..*): A child of this Code

**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description



## Referenced By

[Codelist](Codelist.md) (as items)

[Code](Code.md) (as child)

[HierarchicalCode](HierarchicalCode.md) (as code)

[CodeMap](../Mapping/CodeMap.md) (as source)

[CodeMap](../Mapping/CodeMap.md) (as target)

[CodedAttributeValue](../DataStructure/CodedAttributeValue.md) (as value)

[CodedKeyValue](../DataStructure/CodedKeyValue.md) (as value)

[CodedObservation](../DataStructure/CodedObservation.md) (as value)

[EnumeratedAttributeValue](../MetadataStructure/EnumeratedAttributeValue.md) (as value)

[SourceCode](../Mapping/SourceCode.md) (as code)

[TargetCode](../Mapping/TargetCode.md) (as code)


