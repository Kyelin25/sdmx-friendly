
# ProvisionAgreement



Inherits from: [ConstrainableArtefact](ConstrainableArtefact.md)



## Description

Links the DataProvider to the relevant StructureUsage (e.g. DataflowDefinition or MetadataflowDefinition) for which the provider supplies data or metadata. The agreement may constrain the scope of data or metadata that can be provided by means of a Constraint.




## References

**hasAgreement** ([DataProvider](../Base/DataProvider.md) - 1): Association to the DataProvider providing the data.

**controlledBy** ([StructureUsage](../Base/StructureUsage.md) - 0..*): Association to the StructureUsage.

**source** ([Datasource](Datasource.md) - 0..1): Association to a data or metadata source which can process a data or metadata query.

### Inherited

**content** ([ContentConstraint](ContentConstraint.md) - 0..*): Associates the metadata that constrains the content to be found in a data or metadata source linked to the ConstrainableArtefact.

**attachment** ([AttachmentConstraint](AttachmentConstraint.md) - 0..*): Associates the metadata that constrains the valid content of a ConstrainableArtefact to which metadata may be attached.




