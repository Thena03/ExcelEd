---
layout: base
title: Excelerate
permalink: /
---

<main class="flex-1 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 mt-24">

  <!-- Hero Section -->
  <section class="text-center py-16 bg-green-50 rounded-lg shadow-md">
    <h1 class="text-5xl font-bold text-green-800 mb-4">Excelerate</h1>
    <p class="text-xl text-green-700 mb-8">Your free, open notebook for learning Excel. Use interactive lessons and examples at your own pace.</p>
    <div class="flex justify-center gap-6">
      <a href="{{ '/lessons' | relative_url }}" 
         class="bg-green-700 text-white px-6 py-3 rounded-lg shadow hover:bg-green-600 transition">
         Start Learning
      </a>
      <a href="{{ '/lessons' | relative_url }}" 
         class="bg-green-100 text-green-800 px-6 py-3 rounded-lg shadow hover:bg-green-200 transition">
         Browse Topics
      </a>
    </div>
  </section>

  <!-- Featured Lessons -->
  <section class="mt-16">
    <h2 class="text-3xl font-bold text-green-800 mb-6 text-center">Featured Lessons</h2>
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
      {% assign lesson_pages = site.pages 
         | where_exp: "p", "p.path contains 'Lessons/'" 
         | where_exp: "p", "p.path != 'Lessons/lessonpage.md'" 
         | sort: "order" 
         | slice: 0,6 %} <!-- Show first 6 lessons -->

      {% for lesson in lesson_pages %}
        <a href="{{ lesson.url | relative_url }}" 
           class="block bg-white rounded-xl shadow-sm border border-green-100 p-6 hover:shadow-md hover:bg-green-50 transition">
          <h3 class="text-xl font-semibold text-green-800 mb-2">{{ lesson.title }}</h3>
          {% if lesson.description %}
            <p class="text-green-700 text-sm">{{ lesson.description }}</p>
          {% endif %}
        </a>
      {% endfor %}
    </div>
  </section>

  <!-- What You’ll Learn -->
  <section class="mt-16 text-center">
    <h2 class="text-3xl font-bold text-green-800 mb-6">What You’ll Learn</h2>
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6">
      <div class="bg-green-50 p-6 rounded-lg shadow">
        <h3 class="font-semibold text-green-800 mb-2">Excel Basics</h3>
        <p class="text-green-700 text-sm">Cells, sheets, ribbons, navigation</p>
      </div>
      <div class="bg-green-50 p-6 rounded-lg shadow">
        <h3 class="font-semibold text-green-800 mb-2">Functions & Formulas</h3>
        <p class="text-green-700 text-sm">SUM, IF, VLOOKUP, COUNTIFS, and more</p>
      </div>
      <div class="bg-green-50 p-6 rounded-lg shadow">
        <h3 class="font-semibold text-green-800 mb-2">Data Cleaning</h3>
        <p class="text-green-700 text-sm">Filters, remove duplicates, flash fill</p>
      </div>
      <div class="bg-green-50 p-6 rounded-lg shadow">
        <h3 class="font-semibold text-green-800 mb-2">Charts & Visualization</h3>
        <p class="text-green-700 text-sm">Bar charts, line charts, formatting tips</p>
      </div>
    </div>
  </section>

  <!-- About Section -->
  <section class="mt-16 text-center bg-green-50 p-8 rounded-lg shadow">
    <h2 class="text-3xl font-bold text-green-800 mb-4">Why Excelerate?</h2>
    <p class="text-green-700 max-w-2xl mx-auto">
      Excelerate is a free resource for students, professionals, and everyday learners to build real Excel skills. 
      Start at the beginning or jump straight to the topic you need.
    </p>
  </section>

  <!-- How to Use Section 
  <section class="mt-16 text-center">
    <h2 class="text-3xl font-bold text-green-800 mb-6">How to Use This Open Book</h2>
    <ul class="max-w-2xl mx-auto text-green-700 list-disc list-inside space-y-2 text-left">
      <li>No logins or accounts required</li>
      <li>Jump to any lesson at any time</li>
      <li>Each lesson has Previous / Next buttons for easy navigation</li>
      <li>Fully responsive — works on desktop and mobile</li>
    </ul>
  </section> -->

  <!-- Call-to-Action -->
  <section class="mt-16 text-center mb-16">
    <a href="{{ '/lessons' | relative_url }}" 
       class="bg-green-700 text-white px-8 py-4 rounded-lg shadow hover:bg-green-600 transition text-lg">
       Start Learning Excel
    </a>
  </section>

</main>
