---
layout: lesson
title: Introduction to Excel Math
order: 1
---
<h1 class="text-4xl font-semibold text-center mb-4"> Arithmetic Operations</h1>
<br>
<div class="bg-blue-50 border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h2 class="text-2xl font-semibold text-center mb-4">Learning Objectives:</h2>
<ul class="list-disc list-inside">
<li>  </li>
<li> Learning the how to utilize common arithmetic operations in Excel. </li>
<li> Learning how to use absolute reference when using arithmetic operations. </li>

</ul>
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm"> 
<h2 class="text-2xl font-semibold text-center mb-4"> Addition Operators</h2>
Addition uses the + symbol in Excel in order to add cell values together. This can be used either with the + symbol or by using the SUM function. 
<br> <br>
<p align="center">
  <img src="{{ '/static/sum-math.png' | relative_url }}" alt="Excel Addition example"/> </p>
<br>
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm"> 
<h2 class="text-2xl font-semibold text-center mb-4"> Subtraction Operators</h2>
Subtraction uses the - operator to subtract cell values.  <br><br>
<p align="center">
  <img src="{{ '/static/subtract.png' | relative_url }}" alt="Excel Subtraction example"/> </p>
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm"> 
<h2 class="text-2xl font-semibold text-center mb-4"> Multiplication Operators</h2>
To multiply cell values, use the * symbol in Excel. <br><br>
<p align="center">
  <img src="{{ '/static/multiply.png' | relative_url }}" alt="Excel Multiplication example"/> </p>
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm"> 
<h2 class="text-2xl font-semibold text-center mb-4"> Multiplying Using Absolute Reference</h2>
<br>
You can also use absolute reference to lock a cell and multiply it with other cells.

How to do it, step by step:
<ul class="list-disc list-inside">
<li> Select a cell and type (=) </li>
<li> Select the cell you want to lock and add two dollar signs ($) before the column and row </li>
<li> Type (*) </li>
<li> Select another cell </li>
<li> Hit enter </li>
<li> Fill the range </li>
</ul>
<br> <br>
Example Scenario: Cell B1 contains a tax rate (e.g., 0.06). Column A contains item prices.
You have prices in column A and a fixed tax rate in cell B1. You want to calculate the price of the items with the tax.
<br><br>
Formula: =A2*$B$1
<br><br>
What happens? Excel multiplies 50 by the locked tax rate (0.06). When you drag the formula down, $B$1 stays the same.
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm"> 
<h2 class="text-2xl font-semibold text-center mb-4"> Division Operator</h2>
Division uses the / symbol in Excel. 
<p align="center">
  <img src="{{ '/static/divide.png' | relative_url }}" alt="Excel Division example"/> </p>
  </div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm"> 
<h2 class="text-2xl font-semibold text-center mb-4"> Dividing Using Absolute Reference</h2>
You can also use absolute reference to lock a cell and divide it with other cells.

How to do it, step by step:
<ol class="list-decimal list-inside">
<li> Select a cell and type (=) </li>
<li> Select the cell you want to lock and add two dollar signs ($) before the column and row </li>
<li> Type (/) </li>
<li> Select another cell </li>
<li> Hit enter </li>
<li> Fill the range </li>
</ol>
<br><br>
Mini Example: You want to calculate the percentage of a total value.
<br><br>
Formula: =A2/$B$1
<br><br>
What happens? Excel divides 20 by the locked total (100). When filled down, $B$1 never changes.
<br>
</div>


