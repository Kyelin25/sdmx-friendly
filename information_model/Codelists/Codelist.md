
# Codelist

Inherits from: [ItemScheme](../Base/ItemScheme.md)



## Description

A list from which some statistical concepts (coded concepts) take their values.


## Attributes

**isPartial** (*bool*): Denotes whether the ItemScheme contains a sub set of the full set of Items in the maintained scheme.

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


