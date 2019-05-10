
# OtherNonEnumeratedAttributeValue



Inherits from: [NonEnumeratedAttributeValue](NonEnumeratedAttributeValue.md)



## Description

The value of a ReportedAttribute where the content is not of human-readable text.


## Attributes

### Inherited

**value** (*string*): A text string that is consistent in format to that defined in the Representation of the MetadataAttribute for which this is a ReportedAttribute.



## References

### Inherited

**valueFor** ([MetadataAttribute](MetadataAttribute.md) - 1): Association to the MetadataAttribute in the MetadataStructureDefinition that identifies the Concept and allowed Representation for the ReportedAttribute. Note that this is a conceptual association showing the link to the MetadataStructureDefinition construct. The syntax for the ReportedAttribute will state, in some form, the id of the MetadataAttribute.

**child** ([ReportedAttribute](ReportedAttribute.md) - 0..*): Association to a child ReportedAttribute consistent with the hierarchy defined in the ReportStructure for the MetadataAttribute for which this child is a ReportedAttribute.




