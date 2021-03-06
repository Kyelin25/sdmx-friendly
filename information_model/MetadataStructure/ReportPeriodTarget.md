
# ReportPeriodTarget



Inherits from: [TargetObject](TargetObject.md)



## Description

The target is a report period. Note that this does not describe the use of an object, but rather serves as a unique metadata key for metadata reports. Metadata reports attached to a particular object may vary over time, and this time identifier component can be used to disambiguate the reports, much like the TimeDimension disambiguates Observations in a data series.


## Attributes

### Inherited

**id** (*string*): The unique identifier of the object.

**uri** (*Url*): Universal resource identifiers that may or may not be resolvable.

**urn** (*Urn*): Universal resource name - this is for use in registries: all registered objects have a urn.



## References

### Inherited

**conceptIdentity** ([Concept](../ConceptScheme/Concept.md) - 1): An association to the Concept which carries the values of the measures.

**localRepresentation** ([Representation](../Base/Representation.md) - 1): Associates a Representation to the TargetObject that must be respected when the object is identified in any MetadataSet. This may be enumerated or non-enumerated.

**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description




