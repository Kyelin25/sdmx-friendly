
# ConceptSchemeMap

Inherits from: [ItemSchemeMap](ItemSchemeMap.md)



## Description

Associates a source and target ConceptScheme.


## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

**source** ([ConceptScheme](../ConceptSchemes/ConceptScheme.md) - 1): Association to the source ConceptScheme.

**target** ([ConceptScheme](../ConceptSchemes/ConceptScheme.md) - 1): Association to the target ConceptScheme.

**ItemAssociation** ([ConceptMap](ConceptMap.md) - 1..*): Association to the ItemAssociation.

**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description




