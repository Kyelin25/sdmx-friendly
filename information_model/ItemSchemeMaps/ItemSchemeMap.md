
# ItemSchemeMap

Inherits from: [NameableArtefact](../Base/NameableArtefact.md)

## Subclasses

[ConceptSchemeMap](ConceptSchemeMap.md)

[CodelistMap](CodelistMap.md)

[CategorySchemeMap](CategorySchemeMap.md)

[OrganisationSchemeMap](OrganisationSchemeMap.md)

[ReportingTaxonomyMap](ReportingTaxonomyMap.md)



## Description

Associates two ItemSchemes.


## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

source: [ItemScheme](../Base/ItemScheme.md) (One) - Association to the source ItemScheme.

target: [ItemScheme](../Base/ItemScheme.md) (One) - Association to the target ItemScheme.

ItemAssociation: [ItemAssociation](ItemAssociation.md) (OneOrMany) - Association to the ItemAssociation.

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[StructureSet](../StructureMaps/StructureSet.md) (as itemSchemeMap)

[SchemeMap](../StructureMaps/SchemeMap.md) (as contains)


