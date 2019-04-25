
# Codelist

Inherits from: [ItemScheme](../Base/ItemScheme.md)



## Description

A list from which some statistical concepts (coded concepts) take their values.


## Attributes

isPartial: bool

final: bool

isExternalReference: bool

serviceUrl: Url

structureUrl: Url

version: string

validFrom: Date

validTo: Date

id: string

uri: Url

urn: Urn



## References

items: [Code](Code.md) (ZeroOrMany) - Association to the Codes in the Codelist.

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[CodelistMap](../ItemSchemeMaps/CodelistMap.md) (as source)

[CodelistMap](../ItemSchemeMaps/CodelistMap.md) (as target)

[SourceCodelist](../HybridCodelistMap/SourceCodelist.md) (as codelist)

[TargetCodelist](../HybridCodelistMap/TargetCodelist.md) (as codelist)


