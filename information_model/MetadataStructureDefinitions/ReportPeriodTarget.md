
# ReportPeriodTarget

Inherits from: [TargetObject](TargetObject.md)



The target is a report period. Note that this does not describe the use of an object, but rather serves as a unique metadata key for metadata reports. Metadata reports attached to a particular object may vary over time, and this time identifier component can be used to disambiguate the reports, much like the TimeDimension disambiguates Observations in a data series.

## Attributes

id: string

uri: Url

urn: Urn



## References

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description

conceptIdentity: [Concept](../ConceptSchemes/Concept.md) (One) - No description

localRepresentation: [Representation](../Base/Representation.md) (One) - Associates a Representation to the TargetObject that must be respected when the object is identified in any MetadataSet. This may be enumerated or non-enumerated.



