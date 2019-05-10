
# ReportedAttribute





## Subclasses

[NonEnumeratedAttributeValue](NonEnumeratedAttributeValue.md)

[EnumeratedAttributeValue](EnumeratedAttributeValue.md)



## Description

The value for a MetadataAttribute.




## References

**valueFor** ([MetadataAttribute](MetadataAttribute.md) - 1): Association to the MetadataAttribute in the MetadataStructureDefinition that identifies the Concept and allowed Representation for the ReportedAttribute. Note that this is a conceptual association showing the link to the MetadataStructureDefinition construct. The syntax for the ReportedAttribute will state, in some form, the id of the MetadataAttribute.

**child** ([ReportedAttribute](ReportedAttribute.md) - 0..*): Association to a child ReportedAttribute consistent with the hierarchy defined in the ReportStructure for the MetadataAttribute for which this child is a ReportedAttribute.

### Inherited



## Referenced By

[ReportedAttribute](ReportedAttribute.md) (as child)

[NonEnumeratedAttributeValue](NonEnumeratedAttributeValue.md) (as child)

[XHTMLAttributeValue](XHTMLAttributeValue.md) (as child)

[TextAttributeValue](TextAttributeValue.md) (as child)

[OtherNonEnumeratedAttributeValue](OtherNonEnumeratedAttributeValue.md) (as child)

[EnumeratedAttributeValue](EnumeratedAttributeValue.md) (as child)

[MetadataReport](MetadataReport.md) (as metadata)


