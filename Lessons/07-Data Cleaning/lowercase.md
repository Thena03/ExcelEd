---
layout: lesson
title: Common Data Cleaning Functions
order: 2
---
<div class="bg-blue-50 border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h2 class="text-2xl font-semibold text-center mb-4">Learning Objectives:</h2>
<ul class="list-disc list-inside">
<li>  </li>
<li> Learning how to change capitalization in Excel. </li>
<li> Learning to clean data based on logical functions (True or False).</li>
<li> Understanding the TRIM Function in Excel.</li>
</ul>
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h2 class="text-2xl font-semibold text-center mb-4"> Lower Function</h2>
This function is used to lowercase text in a cell. Changing the letter case of your cell values can be beneficial when there are case inconsistencies among the cell inputs or when preparing your dataset for case-sensitive usage.
<br><br>
It is typed =LOWER <br> <br>
<p align="center">
  <img src="{{ '/static/lowercase.png' | relative_url }}" alt="Excel Lowercase example"/>
</p> <br>
</div> <br>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h2 class="text-2xl font-semibold text-center mb-4"> TRIM Function</h2>
This function is used to remove irregular text spacing and keep single spaces between words.
<br><br>
It is typed =TRIM <br><br>
<p align="center">
  <img src="{{ '/static/TRIM.png' | relative_url }}" alt="Excel Trim example"/>
</p> <br>
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h2 class="text-2xl font-semibold text-center mb-4"> XOR Function</h2>
This function returns TRUE or FALSE based on two or more conditions.
<br><br>
It is typed =XOR
<br><br>
=XOR([logical1], [logical2], ...)
<br><br>
The conditions are referred to as [logical1], [logical2], and so on.
The conditions can check things like:
<ul class="list-disc list-inside">
<li> If a number is greater than another number > </li>
<li> If a number is smaller than another number < </li>
<li> If a number or text is equal to something = </li>
</ul>
<br>
For two conditions, you can think of the XOR function as: "either this or that, but not both" <br><br>
<p align="center">
  <img src="{{ '/static/XOR.png' | relative_url }}" alt="Excel XOR example"/>
</p> <br>
</div>
