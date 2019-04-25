
# ReportingCategory

Inherits from: [Item](../Base/Item.md)



## Description

A component that gives structure to the report and links to data and metadata.


## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.

### Inherited



## References

**flow** ([StructureUsage](../Base/StructureUsage.md) - 0..*): Association to the DataflowDefinitions and MetadataflowDefinitions that link to metadata about the provisioning and related data and metadata sets, and the structures that define them.

**structure** ([Structure](../Base/Structure.md) - 0..*): Association to the DataStructureDefinitions and MetadataStructureDefinitions which define the structural metadata describing the data and metadata that are contained at this part of the report.

### Inherited

**child** ([ReportingCategory](ReportingCategory.md) - 0..*): A child of this ReportingCategory
**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.
**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.
**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description


## Referenced By

[ReportingTaxonomy](ReportingTaxonomy.md) (as items)

[ReportingCategory](ReportingCategory.md) (as child)

[ReportingCategoryMap](../ItemSchemeMaps/ReportingCategoryMap.md) (as source)

[ReportingCategoryMap](../ItemSchemeMaps/ReportingCategoryMap.md) (as target)


