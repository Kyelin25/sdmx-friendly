
# AttributeValue



## Subclasses

[UncodedAttributeValue](UncodedAttributeValue.md)

[CodedAttributeValue](CodedAttributeValue.md)



## Description

The value of an attribute, such as the instance of a Coded Attribute or of an Uncoded Attribute in a structure such as a DataStructureDefinition.


## Attributes

**value** (*string*): The value of the attribute.



## References

**valueFor** ([DataAttribute](DataAttribute.md) - 1): Association to the DataAttribute defined in the DataStructureDefinition. Note that this is a conceptual association as the Concept is identified explicitly in the DataSet.



## Referenced By

[Key](Key.md) (as attachedAttribute)

[GroupKey](GroupKey.md) (as attachedAttribute)

[SeriesKey](SeriesKey.md) (as attachedAttribute)

[Observation](Observation.md) (as attachedAttribute)

[DataSet](DataSet.md) (as attachedAttribute)

[GenericDataSet](GenericDataSet.md) (as attachedAttribute)

[StructureSpecificDataSet](StructureSpecificDataSet.md) (as attachedAttribute)

[GenericTimeseriesDataSet](GenericTimeseriesDataSet.md) (as attachedAttribute)

[StructureSpecificTimeseriesDataSet](StructureSpecificTimeseriesDataSet.md) (as attachedAttribute)


