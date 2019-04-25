
# EnumeratedAttributeValue

Inherits from: [ReportedAttribute](ReportedAttribute.md)



## Description

The content of a ReportedAttribute that is taken from a Code in a Codelist.


## Attributes

value: string



## References

value: [Code](../Codelists/Code.md) (One) - Association to a Code in the Codelist specified in the Representation of the MetadataAttribute for which this ReportedAttribute is the value. Note that this shows the conceptual link to the Item that is the value. In reality the value itself will be contained in the EnumeratedAttributeValue.

valueFor: [MetadataAttribute](MetadataAttribute.md) (One) - Association to the MetadataAttribute in the MetadataStructureDefinition that identifies the Concept and allowed Representation for the ReportedAttribute. Note that this is a conceptual association showing the link to the MetadataStructureDefinition construct. The syntax for the ReportedAttribute will state, in some form, the id of the MetadataAttribute.

child: [ReportedAttribute](ReportedAttribute.md) (ZeroOrMany) - Association to a child ReportedAttribute consistent with the hierarchy defined in the ReportStructure for the MetadataAttribute for which this child is a ReportedAttribute.




