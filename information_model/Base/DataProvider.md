
# DataProvider



Inherits from: [Organisation](Organisation.md), [ConstrainableArtefact](../Registry/ConstrainableArtefact.md)



## Description

An organisation that produces data or reference metadata.


## Attributes

### Inherited

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

### Inherited

**contact** ([Contact](Contact.md) - 1): Association to the Contact information.

**child** ([DataProvider](DataProvider.md) - 0..*): A child of this DataProvider.

**name** ([InternationalString](InternationalString.md) - 1): A multi-lingual name is provided by this role via the InternationalString class.

**description** ([InternationalString](InternationalString.md) - 0..1): A multi-lingual description is provided by this role via the InternationalString class.

**contains** ([Annotation](Annotation.md) - 0..*): No description

**content** ([ContentConstraint](../Registry/ContentConstraint.md) - 0..*): Associates the metadata that constrains the content to be found in a data or metadata source linked to the ConstrainableArtefact.

**attachment** ([AttachmentConstraint](../Registry/AttachmentConstraint.md) - 0..*): Associates the metadata that constrains the valid content of a ConstrainableArtefact to which metadata may be attached.



## Referenced By

[DataProviderScheme](DataProviderScheme.md) (as items)

[DataProvider](DataProvider.md) (as child)

[MetadataSet](../MetadataStructure/MetadataSet.md) (as publishedBy)

[DataSet](../DataStructure/DataSet.md) (as publishedBy)

[GenericDataSet](../DataStructure/GenericDataSet.md) (as publishedBy)

[StructureSpecificDataSet](../DataStructure/StructureSpecificDataSet.md) (as publishedBy)

[GenericTimeseriesDataSet](../DataStructure/GenericTimeseriesDataSet.md) (as publishedBy)

[StructureSpecificTimeseriesDataSet](../DataStructure/StructureSpecificTimeseriesDataSet.md) (as publishedBy)

[ProvisionAgreement](../Registry/ProvisionAgreement.md) (as hasAgreement)


