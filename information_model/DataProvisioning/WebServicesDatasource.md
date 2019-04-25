
# WebServicesDatasource

Inherits from: [Datasource](Datasource.md), [ConstrainableArtefact](../Constraints/ConstrainableArtefact.md)

## Subclasses

[RESTDatasource](RESTDatasource.md)

[SOAPDatasource](SOAPDatasource.md)



## Description

A data or reference metadata source which can process a data or metadata query.


## Attributes

WSDLURL: Url

sourceURL: Url



## References

content: [ContentConstraint](../Constraints/ContentConstraint.md) (ZeroOrMany) - Associates the metadata that constrains the content to be found in a data or metadata source linked to the ConstrainableArtefact.

attachment: [AttachmentConstraint](../Constraints/AttachmentConstraint.md) (ZeroOrMany) - Associates the metadata that constrains the valid content of a ConstrainableArtefact to which metadata may be attached.




