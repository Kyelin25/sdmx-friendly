
# TimeDimensionValue







## Description

Contains identification of the TimeDimension and the value.


## Attributes

### Inherited

**timeValue** (*ObservationalTimePeriod*): The value of the time period.

**operator** (*string*): Indicates whether the specified value represents the exact time or time period, or whether the value should be handled as a range. A value of greaterThan or greaterThanOrEqual indicates that the value is the beginning of a range (exclusive or inclusive, respectively). A value of lessThan or lessThanOrEqual indicates that the value is the end of a range (exclusive or inclusive, respectively). In the absence of the oppositve bound being specified for the range, this bound is to be treated as infinite (e.g. any time period after the beginning of the provided time period for greaterThanOrEqual).





## Referenced By

[ComponentValue](ComponentValue.md) (as contains)


