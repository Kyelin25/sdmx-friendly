
# ItemSchemeMap

Inherits from: [NameableArtefact](../Base/NameableArtefact.md)

## Subclasses

[ConceptSchemeMap](ConceptSchemeMap.md)

[CodelistMap](CodelistMap.md)

[CategorySchemeMap](CategorySchemeMap.md)

[OrganisationSchemeMap](OrganisationSchemeMap.md)

[ReportingTaxonomyMap](ReportingTaxonomyMap.md)



Associates two ItemSchemes.

## Attributes

id: string

uri: Url

urn: Urn



## References

source: [ItemScheme](../Base/ItemScheme.md) (One) - Association to the source ItemScheme.

target: [ItemScheme](../Base/ItemScheme.md) (One) - Association to the target ItemScheme.

ItemAssociation: [ItemAssociation](ItemAssociation.md) (OneOrMany) - Association to the ItemAssociation.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.



## Referenced By

[StructureSet](../StructureMaps/StructureSet.md) (as itemSchemeMap)

[SchemeMap](../StructureMaps/SchemeMap.md) (as contains)


