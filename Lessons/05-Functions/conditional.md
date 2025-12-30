---
layout: lesson
title: Conditional Functions
order: 2
---
<h1 class="text-4xl font-bold text-center mb-4"> Conditional Functions </h1>

<div class="bg-blue-50 border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h2 class="text-2xl font-semibold text-center mb-4">Learning Objectives:</h2>
<ul class="list-disc list-inside">
<li> Learning what IF and IFS Functions are. </li>
<li> Learning what OR and AND Functions are. </li>
<li> Understanding common statistical functions. </li>
</ul>
</div>
<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h2 class="text-2xl font-semibold text-center mb-4"> IF Functions </h2>
This function returns cell values as specified by a true or false condition. It is typed as `=IF` and has three components. <br><br>

=IF(logical_test, [value_if_true], [value_if_false])
The condition is referred to as logical_test, which can check things like: <br>
<ul class="list-disc list-inside">
<li>If a number is greater than another number > </li>
<li>If a number is smaller than another number < </li>
<li>If a number or text is equal to something = </li>
</ul>
<br><br>

<strong>Example: =IF(A2>=70,"Pass","Fail")</strong> <br> <br> If the value in cell A2 is 70 or higher, Excel returns Pass; otherwise, it returns Fail.
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> IFS Functions </h3>
This function returns cell values as specified by multiple true or false condition. It is typed as `=IFS` and has two or more components. <br> <br>

=IFS(logical_test1, value_if_true1, [logical_test2, value_if_true2], [logical_test3]; ...) <br><br>
The condition is referred to as logical_test, which can check things like: 
<ul class="list-disc list-inside">
<li>If a number is greater than another number > </li>
<li>If a number is smaller than another number < </li>
<li>If a number or text is equal to something = </li>
</ul>
<br><br>
<strong>Example: =IFS(A2 >= 90,"A", A2 >= 80,"B", A2 >= 70,"C", A2 < 70,"F")</strong> <br><br> This function will assign a letter grade based on the value in cell A2.
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> OR Functions </h3>
This function returns true or false based on two or more conditions. It is typed as `=OR` =OR([logical1], [logical2], ...). This is often used with the IF function. <br><br>
The condition is referred to as logical1, which can check things like:
<ul class="list-disc list-inside">
<li>If a number is greater than another number > </li>
<li>If a number is smaller than another number < </li>
<li>If a number or text is equal to something = </li>
</ul>
<br><br>

<strong> Example: =IF(OR(A2 < 60, B2="Yes"),"At Risk","OK") 
</strong> <br><br>
Returns At Risk if the score is below 60 or attendance is marked "Yes".
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> AND Functions </h3>
The AND function is a function that returns TRUE or FALSE based on two or more conditions.
<br><br>
<strong> Example: =IF(AND(A2 >= 70, B2 >= 80),"Eligible","Not Eligible") </strong> 
<br><br> Returns "Eligible" only if both conditions are met.

</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> AVERAGEIF Functions </h3>
The AVERAGEIF function calculates the average of a range based on a  TRUE or FALSE condition. It is typed as `=AVERAGEIF`. The syntax for this is
<br><br>
=AVERAGEIF(range, criteria, [average_range])
<br><br>
The condition is referred to as criteria, which can check things like:
<ul class="list-disc list-inside">
<li>If a number is greater than another number > </li>
<li>If a number is smaller than another number < </li>
<li>If a number or text is equal to something = </li>
</ul> <br>
The [average_range] is the range where the function calculates the average.
<br><br>
<strong> Example: =AVERAGEIF(A2:A20,">= 70") </strong> <br> <br> Calculates the average of all values that are 70 or higher.
<br><br>
<strong>Note:</strong> The [average_range] function is optional. If no range is specified, Excel will calculate the average of all the values that fit the criteria. 
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> AVERAGEIFS Functions </h3>
The AVERAGEIFS function calculates the average of a range based on multiple TRUE or FALSE conditions. It is typed as `=AVERAGEIF`. The syntax for this is <br><br>

=AVERAGEIF(average_range, criteria_range1, criteria1, … ) <br><br>

The condition is referred to as criteria, which can check things like:
<ul class="list-disc list-inside">
<li>If a number is greater than another number > </li>
<li>If a number is smaller than another number < </li>
<li>If a number or text is equal to something = </li>
</ul>
<br>
The [average_range] is the range where the function calculates the average. The criteria ranges are the ranges where the function check for the conditions. 
<br><br>
<strong> Example: =AVERAGEIFS(C2:C20, A2:A20,"Running", B2:B20,"> 60") </strong> <br><br> This function calculates the average heart rate for running sessions where speed was 60 or higher.
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> COUNTIF Functions </h3>
This function counts cells as specified by a true or false condition. It is typed as `=COUNTIF`. <br><br>
<strong> Example: =COUNTIF(A2:A30,"Absent") </strong> <br><br> This counts how many times "Absent" appears in the range.
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> COUNTIFS Functions </h3>
This function counts cells as specified by multiple true or false conditions. It is typed as `=COUNTIFS`.
<br><br>
=COUNTIFS(criteria_range1, criteria1, [criteria_range2, criteria2], ...)
<br><br>
<strong> Example: =COUNTIFS(A2:A30,"Female", B2:B30,">=80") </strong> <br><br> This counts how many female athletes scored 80 or higher.

</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> SUMIF Functions </h3>
This function calculates the sum of values in a range based on a true or false condition. <br>
It is typed =SUMIF:
=SUMIF(range, criteria, [sum_range])
<br><br>
The condition is referred to as criteria, which can check things like:
<ul class="list-disc list-inside">
<li>If a number is greater than another number > </li>
<li>If a number is smaller than another number < </li>
<li>If a number or text is equal to something = </li>
</ul>
<br><br>
The [sum_range] is the range where the function calculates the sum.
<br><br>
<strong> Example: =SUMIF(A2:A20,"Equipment",B2:B20) </strong> <br><br> This function adds up all costs in B2:B20 where the categor in A2:A20 is "Equipment."
<br><br>
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> SUMIFS Functions </h3>
This function calculates the sum of values in a range based on a true or false condition. <br><br>
It is typed =SUMIFS:<br><br>
=SUMIFS(sum_range, criteria_range1, criteria1, [criteria_range2, criteria2] ...)
The condition is referred to as criteria_range1, which can check things like:
<ul class="list-disc list-inside">
<li>If a number is greater than another number > </li>
<li>If a number is smaller than another number < </li>
<li>If a number or text is equal to something = </li>
</ul>
<br>
The criteria_range1, criteria_range2, and so on, are the ranges where the function checks for the conditions.
<br><br>
The [sum_range] is the range where the function calculates the sum.
<br><br>
<strong> Example: =SUMIFS(C2:C20, A2:A20,"Running", B2:B20,">=30") </strong> <br><br> This function calculates total distance for running sessions lasting 30 minutes or more.
</div>
