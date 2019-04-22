
# ReportingYearStartDay

Inherits from: [DataAttribute](DataAttribute.md)



A specialised DataAttribute whose value is used in conjunction with the predefined reporting periods in the TimeDimension. If this is not present, then by default all reporting perio values for the TimeDimension will be assumed to be based on a reporting year start day of January 1.

## Attributes

id: string

uri: Url

urn: Urn

usageStatus: UsageStatus



## References

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

conceptIdentity: [Concept](../ConceptSchemes/Concept.md) (One) - No description

localRepresentation: [Representation](../Base/Representation.md) (One) - No description

role: [Concept](../ConceptSchemes/Concept.md) (ZeroOrMany) - Association to the Concept that specifies the role that the DataAttribute plays in the DataStructureDefinition.

relatedTo: [AttributeRelationship](AttributeRelationship.md) (One) - Association to an AttributeRelationship.



