
# ItemScheme

Inherits from: [MaintainableArtefact](MaintainableArtefact.md)

## Subclasses

[Codelist](../Codelists/Codelist.md)



The descriptive information for an arrangement or division of objects into groups based on characteristics, which the objects have in common.

## Attributes

isPartial: bool

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

items: [Item](Item.md) (ZeroOrMany) - Association to the Items in the scheme.

contains: [Annotation](Annotation.md) (ZeroOrMany) - No description

name: [InternationalString](InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

maintainer: [Placeholder](Placeholder.md) (One) - No description



## Referenced By

[Representation](Representation.md) (as enumerated)


