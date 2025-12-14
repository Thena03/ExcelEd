---
layout: lesson
title: Conditional Functions
---
<h1 class="text-4xl font-bold text-center mb-4"> Conditional Functions </h1>


<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h2 class="text-2xl font-semibold text-center mb-4"> IF Functions </h2>
This function returns cell values as specified by a true or false condition. It is typed as `=IF` and has three components. <br>

=IF(logical_test, [value_if_true], [value_if_false])
The condition is referred to as logical_test, which can check things like: <br>
<ul class="list-disc list-inside">
<li>If a number is greater than another number > </li>
<li>If a number is smaller than another number < </li>
<li>If a number or text is equal to something = </li>
</ul>

INSERT EXAMPLE
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> IFS Functions </h3>
This function returns cell values as specified by multiple true or false condition. It is typed as `=IFS` and has two or more components.

=IFS(logical_test1, value_if_true1, [logical_test2, value_if_true2], [logical_test3]; ...) <br>
The condition is referred to as logical_test, which can check things like:
<ul class="list-disc list-inside">
<li>If a number is greater than another number > </li>
<li>If a number is smaller than another number < </li>
<li>If a number or text is equal to something = </li>
</ul>

INSERT EXAMPLE
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> OR Functions </h3>
This function returns true or false based on two or more conditions. It is typed as `=OR` =OR([logical1], [logical2], ...). This is often used with the IF function. <br>
The condition is referred to as logical1, which can check things like:
<ul class="list-disc list-inside">
<li>If a number is greater than another number > </li>
<li>If a number is smaller than another number < </lu>
<li>If a number or text is equal to something = </li>
</ul>
INSERT EXAMPLE
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> AND Functions </h3>
The AND function is a function that returns TRUE or FALSE based on two or more conditions.

Insert example
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> AVERAGEIF Functions </h3>
The AVERAGEIF function calculates the average of a range based on a  TRUE or FALSE condition. It is typed as `=AVERAGEIF`. The syntax for this is
<br>
=AVERAGEIF(range, criteria, [average_range])
<br>
The condition is referred to as criteria, which can check things like:
<ul class="list-disc list-inside">
<li>If a number is greater than another number > </li>
<li>If a number is smaller than another number < </li>
<li>If a number or text is equal to something = </li>
</ul> <br>
The [average_range] is the range where the function calculates the average.

Insert example
</div>

<strong>Note:</strong> The [average_range] function is optional. If no range is specified, Excel will calculate the average of all the values that fit the criteria. 

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> AVERAGEIFS Functions </h3>
The AVERAGEIFS function calculates the average of a range based on multiple TRUE or FALSE conditions. It is typed as `=AVERAGEIF`. The syntax for this is

=AVERAGEIF(average_range, criteria_range1, criteria1, … )

The condition is referred to as criteria, which can check things like:
<ul class="list-disc list-inside">
<li>If a number is greater than another number > </li>
<li>If a number is smaller than another number < </li>
<li>If a number or text is equal to something = </li>
</ul>
<br>
The [average_range] is the range where the function calculates the average. The criteria ranges are the ranges where the function check for the conditions. 
Insert example

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> COUNTIF Functions </h3>
This function counts cells as specified by a true or false condition. It is typed as `=COUNTIF`. <br>
INSERT EXAMPLE
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> COUNTIFS Functions </h3>
This function counts cells as specified by multiple true or false conditions. It is typed as `=COUNTIFS`.
<br>
=COUNTIFS(criteria_range1, criteria1, [criteria_range2, criteria2], ...)
INSERT EXAMPLE
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> SUMIF Functions </h3>
This function calculates the sum of values in a range based on a true or false condition.
It is typed =SUMIF:
=SUMIF(range, criteria, [sum_range])
<br>
The condition is referred to as criteria, which can check things like:
<ul class="list-disc list-inside">
<li>If a number is greater than another number > </li>
<li>If a number is smaller than another number < </li>
<li>If a number or text is equal to something = </li>
</ul>
<br>
The [sum_range] is the range where the function calculates the sum.

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> SUMIFS Functions </h3>
This function calculates the sum of values in a range based on a true or false condition. <br>
It is typed =SUMIFS:
=SUMIFS(sum_range, criteria_range1, criteria1, [criteria_range2, criteria2] ...)
The condition is referred to as criteria_range1, which can check things like:
<ul class="list-disc list-inside">
<li>If a number is greater than another number > </li>
<li>If a number is smaller than another number < </li>
<li>If a number or text is equal to something = </li>
</ul>
<br>
The criteria_range1, criteria_range2, and so on, are the ranges where the function checks for the conditions.
<br>
The [sum_range] is the range where the function calculates the sum.
</div>
