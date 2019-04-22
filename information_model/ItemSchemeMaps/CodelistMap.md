
# CodelistMap

Inherits from: [ItemSchemeMap](ItemSchemeMap.md)



Associates a source and target Codelist.

## Attributes

id: string

uri: Url

urn: Urn



## References

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

source: [Codelist](../Codelists/Codelist.md) (One) - Association to the source Codelist.

target: [Codelist](../Codelists/Codelist.md) (One) - Association to the target Codelist.

ItemAssociation: [ItemAssociation](ItemAssociation.md) (OneOrMany) - Association to the ItemAssociation.




