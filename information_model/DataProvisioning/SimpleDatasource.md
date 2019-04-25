
# SimpleDatasource

Inherits from: [Datasource](Datasource.md), [ConstrainableArtefact](../Constraints/ConstrainableArtefact.md)



## Description

An SDMX-ML Dataset accessible as a file at a URL.


## Attributes

### Inherited

**sourceURL** (*Url*): The URL of the data or reference metadata source (a file or a web service).



## References

### Inherited

**content** ([ContentConstraint](../Constraints/ContentConstraint.md) - 0..*): Associates the metadata that constrains the content to be found in a data or metadata source linked to the ConstrainableArtefact.

**attachment** ([AttachmentConstraint](../Constraints/AttachmentConstraint.md) - 0..*): Associates the metadata that constrains the valid content of a ConstrainableArtefact to which metadata may be attached.




