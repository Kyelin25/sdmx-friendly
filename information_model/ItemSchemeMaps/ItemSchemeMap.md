
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

### Inherited

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

**source** ([ItemScheme](../Base/ItemScheme.md) - 1): Association to the source ItemScheme.

**target** ([ItemScheme](../Base/ItemScheme.md) - 1): Association to the target ItemScheme.

**ItemAssociation** ([ItemAssociation](ItemAssociation.md) - 1..*): Association to the ItemAssociation.

### Inherited

**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description



## Referenced By

[StructureSet](../StructureMaps/StructureSet.md) (as itemSchemeMap)

[SchemeMap](../StructureMaps/SchemeMap.md) (as contains)


