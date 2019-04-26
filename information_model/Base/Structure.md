
# Structure

Inherits from: [MaintainableArtefact](MaintainableArtefact.md)

## Subclasses

[DataStructureDefinition](../DataStructure/DataStructureDefinition.md)

[MetadataStructureDefinition](../MetadataStructure/MetadataStructureDefinition.md)



## Description

Abstract specification of a list of lists to define a complex tabular structure. A concrete example of this would be statistical Concepts, Codelists, and their organisation in a DataStructureDefinition or MetadataStructureDefinition, defined by a central institution, usually for the exchange of statistical information with its partners.


## Attributes

### Inherited

**final** (*bool*): Defines whether a maintained artefact is draft or final.

**isExternalReference** (*bool*): If set to "true" it indicates that the content of the object is held externally.

**serviceUrl** (*Url*): The URL of an SDMX-compliant web service from which the external object can be retrieved.

**structureUrl** (*Url*): The URL of an SDMX-ML document containing the external object

**version** (*string*): A version string following an agreed convention.

**validFrom** (*Date*): Date from which the version is valid.

**validTo** (*Date*): Date from which version is superceded.

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

**grouping** ([ComponentList](ComponentList.md) - 1..*): A composite association to one or more ComponentLists.

### Inherited

**maintainer** ([Agency](Agency.md) - 1): No description

**name** ([InternationalString](InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

**contains** ([Annotation](Annotation.md) - 0..*): No description



## Referenced By

[StructureUsage](StructureUsage.md) (as structure)

[StructureSet](../Mapping/StructureSet.md) (as relatedStructure)

[ReportingCategory](../CategoryScheme/ReportingCategory.md) (as structure)


