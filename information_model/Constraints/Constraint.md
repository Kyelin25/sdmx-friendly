
# Constraint

Inherits from: [MaintainableArtefact](../Base/MaintainableArtefact.md)

## Subclasses

[ContentConstraint](ContentConstraint.md)

[AttachmentConstraint](AttachmentConstraint.md)



## Description

Specifies a subset of the definition of the allowable or actual content of a data or metadata source that can be derived from the Structure that defines Codelists and other valid content.


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

dataContentKeys: [DataKeySet](DataKeySet.md) (ZeroOrMany) - Association to a subset of DataKeySets (i.e. value combinations) that can be derived from the definition of the structure to which the ConstrainableArtefact is linked.

metadataContentKeys: [MetadataKeySet](MetadataKeySet.md) (ZeroOrMany) - Association to a subset of MetadataKeySets (i.e. value combinations) that can be derived from the definition of the Structure to which the ConstrainableArtefact is linked.

role: [ConstraintRole](ConstraintRole.md) (OneOrMany) - Association to the role that the Constraint plays.

maintainer: [Agency](../OrganisationSchemes/Agency.md) (One) - No description

name: [InternationalString](../Base/InternationalString.md) (One) - A multi-lingual name is provided by this role via the InternationalString class.

description: [InternationalString](../Base/InternationalString.md) (ZeroOrOne) - A multi-lingual description is provided by this role via the InternationalString class.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description




