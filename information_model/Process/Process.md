
# Process

Inherits from: [MaintainableArtefact](../Base/MaintainableArtefact.md)



## Description

A scheme which defines or documents the operations performed on data or metadata in order to validate data or metadata to derive new information according to a given set of rules.


## Attributes

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

step: [ProcessStep](ProcessStep.md) (ZeroOrMany) - Associates the ProcessSteps.

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description




