
# FacetType





## Description

Used along with FacetValueType to specify the valid format of the content of a non-enumerated Concept or the usage of a Concept when specified for use on a Component on a Structure.


## Values

**isSequence** (*bool*): The isSequence facet indicates whether the values are intended to be ordered, and it may work in combination with the interval, startValue, and endValue facet or the timeInterval, startTime, and endTime facets. If this attribute holds a value of true, a start value or time and a numeric or time interval must be supplied. If an end value is not given, then the sequence continues indefinitely.

**minLength** (*positiveInteger*): The minLength facet specifies the minimum length of the value in characters.

**maxLength** (*positiveInteger*): The maxLength facet specifies the maximum length of the value in characters.

**minValue** (*decimal*): The minValue facet is used for inclusive and exclusive ranges, indicating what the lower bound of the range is. If this is used with an inclusive range, a valid value will be greater than or equal to the value specified here. If the inclusive and exclusive data type is not specified (e.g. this facet is used with an integer data type), the value is assumed to be inclusive.

**maxValue** (*decimal*): The maxValue facet is used for inclusive and exclusive ranges, indicating what the upper bound of the range is. If this is used with an inclusive range, a valid value will be less than or equal to the value specified here. If the inclusive and exclusive data type is not specified (e.g. this facet is used with an integer data type), the value is assumed to be inclusive.

**startValue** (*decimal*): The startValue facet is used in conjunction with the isSequence and interval facets (which must be set in order to use this facet). This facet is used for a numeric sequence, and indicates the starting point of the sequence. This value is mandatory for a numeric sequence to be expressed.

**endValue** (*string*): The endValue facet is used in conjunction with the isSequence and interval facets (which must be set in order to use this facet). This facet is used for a numeric sequence, and indicates the ending point (if any) of the sequence.

**interval** (*double*): The interval attribute specifies the permitted interval (increment) in a sequence. In order for this to be used, the isSequence attribute must have a value of true.

**timeInterval** (*duration*): The timeInterval facet indicates the permitted duration in a time sequence. In order for this to be used, the isSequence facet must have a value of true.

**decimals** (*positiveInteger*): The decimals facet indicates the number of characters allowed after the decimal separator.

**pattern** (*string*): The pattern attribute holds any regular expression permitted in the implementation syntax (e.g. W3C XML Schema).

**startTime** (*Date*): The startTime facet is used in conjunction with the isSequence and timeInterval facets (which must be set in order to use this facet). This attribute is used for a time sequence, and indicates the start time of the sequence. This value is mandatory for a time sequence to be expressed.

**endTime** (*Date*): The endTime facet is used in conjunction with the isSequence and timeInterval facets (which must be set in order to use this faceet). This facet is used for a time sequence, and indicates the ending point (if any) of the sequence.


