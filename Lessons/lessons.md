---
layout: base
title: Lessons
---

<h1 class="text-3xl font-bold text-green-800 mb-6">Excelerate Lessons</h1>

{% assign lesson_groups = site.Lessons %}
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
  {% for folder in site.Lessons %}
    <div class="bg-green-50 p-4 rounded shadow hover:shadow-lg transition">
      <h2 class="text-xl font-semibold text-green-700 mb-2">{{ folder.name }}</h2>
      <ul class="list-disc list-inside text-green-800">
        {% for lesson in folder.files %}
          <li><a href="{{ lesson.url }}" class="hover:text-green-600">{{ lesson.title }}</a></li>
        {% endfor %}
      </ul>
    </div>
  {% endfor %}
</div>
