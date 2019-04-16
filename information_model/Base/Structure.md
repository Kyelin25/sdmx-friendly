
# Structure

Inherits from: [MaintainableArtefact](MaintainableArtefact.md)



Abstract specification of a list of lists to define a complex tabular structure. A concrete example of this would be statistical Concepts, Codelists, and their organisation in a DataStructureDefinition or MetadataStructureDefinition, defined by a central institution, usually for the exchange of statistical information with its partners.

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

grouping: [ComponentList](ComponentList.md) (OneOrMany) - A composite association to one or more ComponentLists.

contains: [Annotation](Annotation.md) (ZeroOrMany) - No description

name: [InternationalString](InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

maintainer: [Placeholder](Placeholder.md) (One) - No description




