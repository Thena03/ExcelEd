---
layout: lesson
title: NPV Function
order: 6
---

<div class="bg-blue-50 border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h2 class="text-2xl font-semibold text-center mb-4">Learning Objectives:</h2>
<ul class="list-disc list-inside">
<li> Learning the purpose behind the net present value function. </li>
</ul>
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm"> 
<h2 class="text-2xl font-semibold text-center mb-4"> Net Present Value (NPV) Function</h2>
The NPV function calculates the Net Present Value of an investment using a discount rate and a series of future cash flows. The purpose of this function is to help decide whether an investment is positive in the future.
<br><br>
The syntax is:
<br>
= NPV(rate, value 1, value 2,...)
<br><br>
<strong>Rate</strong> = discount rate per period
<strong>Value1, value2… </strong> = series of cash flows occurring at the end of each period 
To use this function, use `=NPV`. 
<br><br>
<p align="center">
  <img src="{{ '/static/NPV.png' | relative_url }}" alt="Excel NPV example"/> </p>
<br><br>
<strong>Note:</strong> The NPV function discounts from the first period, so the initial investment must be added after the function to get the correct total. 
</div>