
# NonEnumeratedAttributeValue

Inherits from: [ReportedAttribute](ReportedAttribute.md)

## Subclasses

[XHTMLAttributeValue](XHTMLAttributeValue.md)

[TextAttributeValue](TextAttributeValue.md)

[OtherNonEnumeratedAttributeValue](OtherNonEnumeratedAttributeValue.md)



The content of a ReportedAttribute where this is textual.



## References

valueFor: [MetadataAttribute](MetadataAttribute.md) (One) - Association to the MetadataAttribute in the MetadataStructureDefinition that identifies the Concept and allowed Representation for the ReportedAttribute. Note that this is a conceptual association showing the link to the MetadataStructureDefinition construct. The syntax for the ReportedAttribute will state, in some form, the id of the MetadataAttribute.

child: [ReportedAttribute](ReportedAttribute.md) (ZeroOrMany) - Association to a child ReportedAttribute consistent with the hierarchy defined in the ReportStructure for the MetadataAttribute for which this child is a ReportedAttribute.



