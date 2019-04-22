
# ContentConstraint

Inherits from: [Constraint](Constraint.md)



Defines a Constraint in terms of the content that can be found in data or metadata sources linked to the ConstrainableArtefact to which this constraint is associated.

## Attributes

id: string

uri: Url

urn: Urn

version: A version string following an agreed convention.

validFrom: Date from which the version is valid.

validTo: Date from which version is superceded.

final: Defines whether a maintained artefact is draft or final.

isExternalReference: If set to "true" it indicates that the content of the object is held externally. 

serviceUrl: The URL of an SDMX-compliant web service from which the external object can be retrieved.

structureUrl: The URL of an SDMX-ML document containing the external object



## References

dataContentRegion: [CubeRegion](CubeRegion.md) (ZeroOrMany) - Association to a subset of Component values that can be derived from the DataStructureDefinition to which the ConstrainableArtefact is linked.

metadataContentRegion: [MetadataTargetRegion](MetadataTargetRegion.md) (ZeroOrMany) - Association to a subset of Component values that can be derived from the MetadataStructureDefinition to which the ConstrainableArtefact is linked.

availableDates: [ReferencePeriod](ReferencePeriod.md) (ZeroOrOne) - Association to the time period that identifies the time range for which data or metadata are available in the data source.

contains: [ReleaseCalendar](ReleaseCalendar.md) (ZeroOrOne) - Association to a ReleaseCalendar

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description

dataContentKeys: [DataKeySet](DataKeySet.md) (ZeroOrMany) - Association to a subset of DataKeySets (i.e. value combinations) that can be derived from the definition of the structure to which the ConstrainableArtefact is linked.

metadataContentKeys: [MetadataKeySet](MetadataKeySet.md) (ZeroOrMany) - Association to a subset of MetadataKeySets (i.e. value combinations) that can be derived from the definition of the Structure to which the ConstrainableArtefact is linked.

role: [ConstraintRole](ConstraintRole.md) (OneOrMany) - Association to the role that the Constraint plays.



## Referenced By

[ConstrainableArtefact](ConstrainableArtefact.md) (as content)


