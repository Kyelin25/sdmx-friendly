
# MeasureKeyValue

Inherits from: [KeyValue](KeyValue.md)



The value of the MeasureDimension component of the Key. The value is the Concept to which this class is associated.



## References

value: [Concept](../ConceptSchemes/Concept.md) (One) - Association to the Concept. Note that this is a conceptual association showing that the Concept must exist in the ConceptScheme associated with the MeasureDimension in the DataStructureDefinition. In the actual DataSet the value of the Concept is placed in the KeyValue.

valueFor: [Dimension](Dimension.md) (One) - Association to the key component in the DataStructureDefinition for which this KeyValue is a valid representation. Note that this is a conceptual association as the key component is identified explicitly in the DataSet.



