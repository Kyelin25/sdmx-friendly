
# CategorySchemeMap

Inherits from: [ItemSchemeMap](ItemSchemeMap.md)



## Description

Associates a source and target CategoryScheme.


## Attributes

id: string

uri: Url

urn: Urn



## References

source: [CategoryScheme](../CategorySchemes/CategoryScheme.md) (One) - Association to the source CategoryScheme.

target: [CategoryScheme](../CategorySchemes/CategoryScheme.md) (One) - Association to the target CategoryScheme.

ItemAssociation: [ConceptMap](ConceptMap.md) (OneOrMany) - Association to the ItemAssociation.

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description




