
# CodedAttributeValue

Inherits from: [AttributeValue](AttributeValue.md)



## Description

An Attribute that takes its value from a Code in a Codelist.


## Attributes

**value** (*string*): The value of the attribute.

### Inherited



## References

### Inherited

**value** ([Code](../Codelists/Code.md) - 1): Association to the Code that is the value of the AttributeValue. Note that this is a conceptual association showing that the Code must exist in the Codelist associated with the DataAttribute in the DataStructureDefinition. In the actual DataSet the value of the Code is placed in the AttributeValue.
**valueFor** ([DataAttribute](DataAttribute.md) - 1): Association to the DataAttribute defined in the DataStructureDefinition. Note that this is a conceptual association as the Concept is identified explicitly in the DataSet.



