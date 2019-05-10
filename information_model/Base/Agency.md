
# Agency



Inherits from: [Organisation](Organisation.md)



## Description

Responsible Agency for maintaining artefacts such as statistical classifications, glossaries, structural metadata such as DataStructureDefinitions and MetadataStructureDefinitions, Concepts and Codelists.


## Attributes

### Inherited

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

### Inherited

**contact** ([Contact](Contact.md) - 1): Association to the Contact information.

**child** ([Agency](Agency.md) - 0..*): A child of this Agency

**name** ([InternationalString](InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

**contains** ([Annotation](Annotation.md) - 0..*): No description



## Referenced By

[MaintainableArtefact](MaintainableArtefact.md) (as maintainer)

[ItemScheme](ItemScheme.md) (as maintainer)

[Codelist](../Codelist/Codelist.md) (as maintainer)

[ConceptScheme](../ConceptScheme/ConceptScheme.md) (as maintainer)

[CategoryScheme](../CategoryScheme/CategoryScheme.md) (as maintainer)

[OrganisationScheme](OrganisationScheme.md) (as maintainer)

[AgencyScheme](AgencyScheme.md) (as items)

[AgencyScheme](AgencyScheme.md) (as maintainer)

[DataProviderScheme](DataProviderScheme.md) (as maintainer)

[DataConsumerScheme](DataConsumerScheme.md) (as maintainer)

[OrganisationUnitScheme](OrganisationUnitScheme.md) (as maintainer)

[ReportingTaxonomy](../CategoryScheme/ReportingTaxonomy.md) (as maintainer)

[Structure](Structure.md) (as maintainer)

[DataStructureDefinition](../DataStructure/DataStructureDefinition.md) (as maintainer)

[MetadataStructureDefinition](../MetadataStructure/MetadataStructureDefinition.md) (as maintainer)

[StructureUsage](StructureUsage.md) (as maintainer)

[DataflowDefinition](../DataStructure/DataflowDefinition.md) (as maintainer)

[MetadataFlowDefinition](../MetadataStructure/MetadataFlowDefinition.md) (as maintainer)

[HierarchicalCodelist](../Codelist/HierarchicalCodelist.md) (as maintainer)

[StructureSet](../Mapping/StructureSet.md) (as maintainer)

[Constraint](../Registry/Constraint.md) (as maintainer)

[ContentConstraint](../Registry/ContentConstraint.md) (as maintainer)

[AttachmentConstraint](../Registry/AttachmentConstraint.md) (as maintainer)

[Process](../Process/Process.md) (as maintainer)

[Agency](Agency.md) (as child)


