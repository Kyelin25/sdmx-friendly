
# ReportingCategory

Inherits from: [Item](../Base/Item.md)



A component that gives structure to the report and links to data and metadata.

## Attributes

id: string

uri: Url

urn: Urn



## References

flow: [StructureUsage](../Base/StructureUsage.md) (ZeroOrMany) - Association to the DataflowDefinitions and MetadataflowDefinitions that link to metadata about the provisioning and related data and metadata sets, and the structures that define them.

structure: [Structure](../Base/Structure.md) (ZeroOrMany) - Association to the DataStructureDefinitions and MetadataStructureDefinitions which define the structural metadata describing the data and metadata that are contained at this part of the report.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

child: [Item](../Base/Item.md) (ZeroOrMany) - A child of this item.



## Referenced By

[ItemScheme](../Base/ItemScheme.md) (as items)

[ItemAssociation](../ItemSchemeMaps/ItemAssociation.md) (as source)

[ItemAssociation](../ItemSchemeMaps/ItemAssociation.md) (as target)


