---
layout: lesson
title: Conditional Functions
---
# Conditional Functions


## IF FUNCTION
This function returns cell values as specified by a true or false condition. It is typed as `=IF` and has three components.

=IF(logical_test, [value_if_true], [value_if_false])
The condition is referred to as logical_test, which can check things like:
If a number is greater than another number >
If a number is smaller than another number <
If a number or text is equal to something =

INSERT EXAMPLE

### IFS FUNCTION
This function returns cell values as specified by multiple true or false condition. It is typed as `=IFS` and has two or more components.

=IFS(logical_test1, value_if_true1, [logical_test2, value_if_true2], [logical_test3; ...)
The condition is referred to as logical_test, which can check things like:
If a number is greater than another number >
If a number is smaller than another number <
If a number or text is equal to something =

INSERT EXAMPLE

## OR FUNCTION
This function returns true or false based on two or more conditions. It is typed as `=OR` =OR([logical1], [logical2], ...). This is often used with the IF function. 
The condition is referred to as logical1, which can check things like:
If a number is greater than another number >
If a number is smaller than another number <
If a number or text is equal to something =
INSERT EXAMPLE

## And Function
The AND function is a function that returns TRUE or FALSE based on two or more conditions.

Insert example

## AVERAGEIF Function
The AVERAGEIF function calculates the average of a range based on a  TRUE or FALSE condition. It is typed as `=AVERAGEIF`. The syntax for this is

=AVERAGEIF(range, criteria, [average_range])

The condition is referred to as criteria, which can check things like:
If a number is greater than another number >
If a number is smaller than another number <
If a number or text is equal to something =
The [average_range] is the range where the function calculates the average.

Insert example

**Note:** The [average_range] function is optional. If no range is specified, Excel will calculate the average of all the values that fit the criteria. 

## AVERAGEIFS Function
The AVERAGEIFS function calculates the average of a range based on multiple TRUE or FALSE conditions. It is typed as `=AVERAGEIF`. The syntax for this is

=AVERAGEIF(average_range, criteria_range1, criteria1, … )

The condition is referred to as criteria, which can check things like:
If a number is greater than another number >
If a number is smaller than another number <
If a number or text is equal to something =

The [average_range] is the range where the function calculates the average. The criteria ranges are the ranges where the function check for the conditions. 
Insert example

## COUNTIF FUNCTION
This function counts cells as specified by a true or false condition. It is typed as `=COUNTIF`.
INSERT EXAMPLE
### COUNTIFS FUNCTION
This function counts cells as specified by multiple true or false conditions. It is typed as `=COUNTIFS`.

=COUNTIFS(criteria_range1, criteria1, [criteria_range2, criteria2], ...)
INSERT EXAMPLE

## SUMIF FUNCTION
This function calculates the sum of values in a range based on a true or false condition.
It is typed =SUMIF:
=SUMIF(range, criteria, [sum_range])

The condition is referred to as criteria, which can check things like:
If a number is greater than another number >
If a number is smaller than another number <
If a number or text is equal to something =

The [sum_range] is the range where the function calculates the sum.
## SUMIFS FUNCTION
This function calculates the sum of values in a range based on a true or false condition.
It is typed =SUMIFS:
=SUMIFS(sum_range, criteria_range1, criteria1, [criteria_range2, criteria2] ...)
The condition is referred to as criteria_range1, which can check things like:
If a number is greater than another number >
If a number is smaller than another number <
If a number or text is equal to something =
The criteria_range1, criteria_range2, and so on, are the ranges where the function checks for the conditions.

The [sum_range] is the range where the function calculates the sum.

