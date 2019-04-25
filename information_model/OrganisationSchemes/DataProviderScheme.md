
# DataProviderScheme

Inherits from: [OrganisationScheme](OrganisationScheme.md)



## Description

A maintained collection of DataProviders.


## Attributes

isPartial: bool

final: Defines whether a maintained artefact is draft or final.

isExternalReference: If set to "true" it indicates that the content of the object is held externally. 

serviceUrl: The URL of an SDMX-compliant web service from which the external object can be retrieved.

structureUrl: The URL of an SDMX-ML document containing the external object

version: A version string following an agreed convention.

validFrom: Date from which the version is valid.

validTo: Date from which version is superceded.

id: string

uri: Url

urn: Urn



## References

items: [DataProvider](DataProvider.md) (ZeroOrMany) - Association to the DataProviders in the DataProviderScheme.

maintainer: [Agency](Agency.md) (One) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description




