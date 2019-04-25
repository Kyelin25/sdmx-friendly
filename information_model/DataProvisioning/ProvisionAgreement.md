
# ProvisionAgreement

Inherits from: [ConstrainableArtefact](../Constraints/ConstrainableArtefact.md)



## Description

Links the DataProvider to the relevant StructureUsage (e.g. DataflowDefinition or MetadataflowDefinition) for which the provider supplies data or metadata. The agreement may constrain the scope of data or metadata that can be provided by means of a Constraint.




## References

hasAgreement: [DataProvider](../OrganisationSchemes/DataProvider.md) (One) - Association to the DataProvider providing the data.

controlledBy: [StructureUsage](../Base/StructureUsage.md) (ZeroOrMany) - Association to the StructureUsage.

source: [Placeholder](../Base/Placeholder.md) (ZeroOrOne) - Association to a data or metadata source which can process a data or metadata query.

content: [ContentConstraint](../Constraints/ContentConstraint.md) (ZeroOrMany) - Associates the metadata that constrains the content to be found in a data or metadata source linked to the ConstrainableArtefact.

attachment: [AttachmentConstraint](../Constraints/AttachmentConstraint.md) (ZeroOrMany) - Associates the metadata that constrains the valid content of a ConstrainableArtefact to which metadata may be attached.




