
# ConstrainableArtefact

*Abstract*



## Subclasses

[DataflowDefinition](../DataStructure/DataflowDefinition.md)

[MetadataFlowDefinition](../MetadataStructure/MetadataFlowDefinition.md)

[DataStructureDefinition](../DataStructure/DataStructureDefinition.md)

[MetadataStructureDefinition](../MetadataStructure/MetadataStructureDefinition.md)

[DataProvider](../Base/DataProvider.md)

[DataSet](../DataStructure/DataSet.md)

[ProvisionAgreement](ProvisionAgreement.md)

[SimpleDatasource](SimpleDatasource.md)

[WebServicesDatasource](WebServicesDatasource.md)



## Description

An artefact that can have Constraints specified.




## References

**content** ([ContentConstraint](ContentConstraint.md) - 0..*): Associates the metadata that constrains the content to be found in a data or metadata source linked to the ConstrainableArtefact.

**attachment** ([AttachmentConstraint](AttachmentConstraint.md) - 0..*): Associates the metadata that constrains the valid content of a ConstrainableArtefact to which metadata may be attached.

### Inherited




