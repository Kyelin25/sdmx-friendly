
# AgencyScheme

Inherits from: [OrganisationScheme](OrganisationScheme.md)



## Description

A maintained collection of Maintenance Agencies.


## Attributes

### Inherited

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

### Inherited

**items** ([Agency](Agency.md) - 0..*): Association to the Agencies in the AgencyScheme.

**maintainer** ([Agency](Agency.md) - 1): No description

**name** ([InternationalString](InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

**contains** ([Annotation](Annotation.md) - 0..*): No description




