
# RESTDatasource

Inherits from: [WebServicesDatasource](WebServicesDatasource.md)



## Description

A data or reference metadata source that is accessible via a RESTful web services interface.


## Attributes

**WSDLURL** (*Url*): Association to the URL of the Web Service Definition Language (SOAP) or Web Service Application Language (REST) profile of the web service.

**sourceURL** (*Url*): The URL of the data or reference metadata source (a file or a web service).

### Inherited



## References

**content** ([ContentConstraint](../Constraints/ContentConstraint.md) - 0..*): Associates the metadata that constrains the content to be found in a data or metadata source linked to the ConstrainableArtefact.

**attachment** ([AttachmentConstraint](../Constraints/AttachmentConstraint.md) - 0..*): Associates the metadata that constrains the valid content of a ConstrainableArtefact to which metadata may be attached.

### Inherited




