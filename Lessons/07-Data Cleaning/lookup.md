---
layout: lesson
title: Searching Functions
order: 3
---
<h1 class="text-4xl font-semibold text-center mb-4"> Searching Functions</h1>
<br>
<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h2 class="text-2xl font-semibold text-center mb-4"> VLOOKUP</h2>
This function allows searches across columns.
<br>
It is typed =VLOOKUP
<br>
=VLOOKUP(lookup_value, table_array, col_index_num, [range_lookup])
<br>
<strong> Lookup_value: </strong> Select the cell where search values will be entered.
<br>
<strong> Table_array: </strong> The table range, including all cells in the table.
<br>
<strong> Col_index_num: </strong> The data that is being looked up. The input is the number of the column, counted from the left: <br><br>
<p align="center">
  <img src="{{ '/static/VLOOKUP.png' | relative_url }}" alt="Excel VLOOKUP example"/>
</p>
<br>
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h2 class="text-2xl font-semibold text-center mb-4"> LEFT Function</h2>
This function is used to retrieve a specified number of characters (ex. letters, numbers, etc.), counting from the left side of an Excel cell. The chosen number has to be greater than 0 and is set to 1 by default.
<br>
It is typed =LEFT <br><br>
<p align="center">
  <img src="{{ '/static/Left.png' | relative_url }}" alt="Excel =LEFT example"/>
</p> <br><br>
In this example, the output would be "numb" since these are the first 4 characters from the left side of the cell.
</div>

<div class="bg-white border-l-4 border-green-600 p-4 rounded-lg mb-6 shadow-sm">
<h2 class="text-2xl font-semibold text-center mb-4"> RIGHT Function</h2>
This function is used to retrieve a specified number of characters, counting from the right side of an Excel cell. The chosen number has to be greater than 0 and is set to 1 by default.
<br>
It is typed =RIGHT <br><br>
<p align="center">
  <img src="{{ '/static/Right.png' | relative_url }}" alt="Excel =RIGHT example"/>
</p>
<br><br>
In this example, the output would be "nges" since these are the first 4 characters from the right side of the cell.
<br>
</div>