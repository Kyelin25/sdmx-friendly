
# Observation

Inherits from: [](..//.md)



The value of the observed phenomenon in the context of the KeyValues comprising the key.



## References

valueFor: [PrimaryMeasure](PrimaryMeasure.md) (One) - Associates the PrimaryMeasure defined in the DataStructureDefinition.

attachedAttribute: [AttributeValue](AttributeValue.md) (ZeroOrMany) - Association to the AttributeValues relating to the Observation.

observationDimension: [KeyValue](KeyValue.md) (One) - Association to the KeyValue that holds the value of the "Dimension at the Observation Level"

contains: [ObservationValue](ObservationValue.md) (One) - The ObservationValue contained in this Observation.



## Referenced By

[SeriesKey](SeriesKey.md) (as contains)


