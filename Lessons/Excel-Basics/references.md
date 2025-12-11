---
layout: lesson
title: Relative v. Absolute References 
---

<h1 class="text-4xl font-semibold text-center mb-4">Relative v. Absolute References</h1>

<div class="bg-blue-50 border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h2 class="text-2xl font-semibold text-center mb-4">Learning Objectives:</h2>
<ul class="list-disc list-inside">
<li> Understanding the difference between relative and absolute references </li>
<li> Understanding the purpose behind relative references </li>
<li> Understanding the purpose behind absolute references </li>
</ul>
</div>
<br>
Cells have unique references (also known as their location in the spreadsheet). The two types of references in Excel are relative references and absolute references. 
<br>
<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h2 class="text-2xl font-semibold text-center mb-4">Relative Reference</h2>
References are relative by default. They are marked without a dollar sign ($). This gives the fill function the freedom to continue the order in a range without restrictions. 
<br>
![Excel Working relative example](/images/ribbon.png)
![Excel error relative example](/images/ribbon.png)
</div>


<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h2 class="text-2xl font-semibold text-center mb-4">Absolute Reference</h2>
An absolute reference is a reference that utilizes a dollar sign. This dollar sign indicates that the cell(s) are locked. 

<strong>The dollar sign has three different states:</strong>
<ul class="list-disc list-inside">
  <li><strong>Column and Row</strong>
  <ul class="list-disc list-inside">
    <li> The reference locks both the column and the row. </li>
    <li><strong>Example:</strong> $A$1</li>
    </ul>

 <li> <strong> Column </strong>
 <ul class="list-disc list-inside">
    <li> The reference is locked to the column. </li>
     <li> The row remains relative (free). </li>
    <li> <strong> Example:</strong> $A1` </li>
    </ul>

  <li> <strong>Row </strong>
  <ul class="list-disc list-inside">
    <li> The reference is locked to the row. </li>
    <li> The column remains relative (free). </li>
    <li> <strong>Example:</strong> A$1 </li>
    </ul>
    </ul>
</div>
