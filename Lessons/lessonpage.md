---
layout: base
title: Lessons
permalink: /lessons/
---

<h1 class="text-2xl font-bold text-green-800 mb-4">Lessons</h1>

{% assign lesson_pages = site.pages | where_exp: "page", "page.path contains 'Lessons/'" %}
{% assign lesson_pages = lesson_pages | where_exp: "page", "page.path != 'Lessons/lessonpage.md'" %}

{% assign lessons_by_folder = lesson_pages | group_by_exp: "page", "page.path | split: '/' | slice: 1" %}
<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 mt-4">
  {% for lesson in folder.items %}
    <a 
      href="{{ lesson.url | relative_url }}" 
      class="block p-4 bg-white rounded-xl shadow hover:shadow-md hover:-translate-y-1 transition transform"
    >
      <h3 class="text-lg font-semibold text-green-800 mb-1">
        {{ lesson.title }}
      </h3>

      {% if lesson.description %}
        <p class="text-gray-600 text-sm">
          {{ lesson.description }}
        </p>
      {% endif %}
    </a>
  {% endfor %}
</div>

