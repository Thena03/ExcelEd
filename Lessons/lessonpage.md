---
layout: base
title: Lessons
permalink: /lessons/
---

<h1 class="text-2xl font-bold text-green-800 mb-4">Lessons</h1>

{% assign lesson_pages = site.pages | where_exp: "page", "page.path contains 'Lessons/'" %}
{% assign lesson_pages = lesson_pages | where_exp: "page", "page.path != 'Lessons/lessonpage.md'" %}

{% assign lessons_by_folder = lesson_pages | group_by_exp: "page", "page.path | split: '/' | slice: 1" %}

{% for folder in lessons_by_folder %}
  <h2 class="text-xl font-semibold text-green-700 mt-6 mb-2">{{ folder.name | capitalize }}</h2>
  <ul class="list-disc list-inside">
    {% for lesson in folder.items %}
      <li>
        <a href="{{ lesson.url | relative_url }}" class="text-green-800 hover:text-green-600">
          {{ lesson.title }}
        </a>
      </li>
    {% endfor %}
  </ul>
{% endfor %}
