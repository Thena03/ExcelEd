---
layout: lesson
title: Creating Formulas
---

<div class="bg-blue-50 border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h3 class="text-xl font-semibold text-center mb-4"> Learning Objectives:</h3>
<ul class="list-disc list-inside">
<li> How to create a formula </li>
<li> Purpose of formulas </li>
</ul>
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h2 class="text-2xl font-semibold text-center mb-4"> Creating a Formula Within a Cell </h2>
You can also create formulas using specific cell values. If cells already have values placed in them. You can select these cells to use them for the formula. Now let’s go through an example.
<br><br>
<p align="center">
  <img src="{{ '/static/creatingaformula.png' | relative_url }}" alt="Excel Creating a Formula example"/>
</p>
In this example, we use the <strong>=</strong> sign to tell Excel that we are going to use a formula in this cell. Then we write the formula (in this case, we are using Excel's built-in addition formula) and select the cells we are going to use in the formula. Then Excel presents the output in the cell. 
<br><br>
This can also be done using the fill operation.
<br><br>
<p align="center">
  <img src="{{ '/static/fill-formulas.png' | relative_url }}" alt="Excel Formulas with fill operation example"/>
</p>
<br><br>
In this example, we are using the sum formula we used in the prior example to calculate the sum of the number of oranges we have. We used the fill operation to drag the cell that contains the formula (the cell with 30 in yellow) and dragged it over to the side next to it so that Excel will calculate the sum of the numbers in the column with oranges. 
<br>
</div>