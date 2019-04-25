
# CodelistMap

Inherits from: [ItemSchemeMap](ItemSchemeMap.md)



## Description

Associates a source and target Codelist.


## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

source: [Codelist](../Codelists/Codelist.md) (One) - Association to the source Codelist.

target: [Codelist](../Codelists/Codelist.md) (One) - Association to the target Codelist.

ItemAssociation: [ConceptMap](ConceptMap.md) (OneOrMany) - Association to the ItemAssociation.

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description




