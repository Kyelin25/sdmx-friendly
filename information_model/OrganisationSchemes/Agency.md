
# Agency

Inherits from: [Organisation](Organisation.md)



## Description

Responsible Agency for maintaining artefacts such as statistical classifications, glossaries, structural metadata such as DataStructureDefinitions and MetadataStructureDefinitions, Concepts and Codelists.


## Attributes

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.

### Inherited



## References

**contact** ([Contact](Contact.md) - 1): Association to the Contact information.

**child** ([Agency](Agency.md) - 0..*): A child of this Agency

**name** ([InternationalString](../Base/InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](../Base/InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description

### Inherited



## Referenced By

[MaintainableArtefact](../Base/MaintainableArtefact.md) (as maintainer)

[ItemScheme](../Base/ItemScheme.md) (as maintainer)

[Codelist](../Codelists/Codelist.md) (as maintainer)

[ConceptScheme](../ConceptSchemes/ConceptScheme.md) (as maintainer)

[CategoryScheme](../CategorySchemes/CategoryScheme.md) (as maintainer)

[OrganisationScheme](OrganisationScheme.md) (as maintainer)

[AgencyScheme](AgencyScheme.md) (as items)

[AgencyScheme](AgencyScheme.md) (as maintainer)

[DataProviderScheme](DataProviderScheme.md) (as maintainer)

[DataConsumerScheme](DataConsumerScheme.md) (as maintainer)

[OrganisationUnitScheme](OrganisationUnitScheme.md) (as maintainer)

[ReportingTaxonomy](../ReportingTaxonomies/ReportingTaxonomy.md) (as maintainer)

[Structure](../Base/Structure.md) (as maintainer)

[DataStructureDefinition](../DataStructureDefinitions/DataStructureDefinition.md) (as maintainer)

[MetadataStructureDefinition](../MetadataStructureDefinitions/MetadataStructureDefinition.md) (as maintainer)

[StructureUsage](../Base/StructureUsage.md) (as maintainer)

[DataflowDefinition](../DataStructureDefinitions/DataflowDefinition.md) (as maintainer)

[MetadataFlowDefinition](../MetadataStructureDefinitions/MetadataFlowDefinition.md) (as maintainer)

[HierarchicalCodelist](../HierarchicalCodelists/HierarchicalCodelist.md) (as maintainer)

[StructureSet](../StructureMaps/StructureSet.md) (as maintainer)

[Constraint](../Constraints/Constraint.md) (as maintainer)

[ContentConstraint](../Constraints/ContentConstraint.md) (as maintainer)

[AttachmentConstraint](../Constraints/AttachmentConstraint.md) (as maintainer)

[Process](../Process/Process.md) (as maintainer)

[Agency](Agency.md) (as child)


