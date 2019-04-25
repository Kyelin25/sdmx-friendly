
# ReportingYearStartDay

Inherits from: [DataAttribute](DataAttribute.md)



## Description

A specialised DataAttribute whose value is used in conjunction with the predefined reporting periods in the TimeDimension. If this is not present, then by default all reporting perio values for the TimeDimension will be assumed to be based on a reporting year start day of January 1.


## Attributes

**usageStatus** (*UsageStatus*): Defines the usage status which is constrained by the data type UsageStatus.

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.

### Inherited



## References

**role** ([Concept](../ConceptSchemes/Concept.md) - 0..*): Association to the Concept that specifies the role that the DataAttribute plays in the DataStructureDefinition.

**relatedTo** ([AttributeRelationship](AttributeRelationship.md) - 1): Association to an AttributeRelationship.

**conceptIdentity** ([Concept](../ConceptSchemes/Concept.md) - 1): No description

**localRepresentation** ([Representation](../Base/Representation.md) - 1): No description

**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description

### Inherited




