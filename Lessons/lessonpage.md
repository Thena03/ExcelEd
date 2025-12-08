---
layout: base
title: Lessons
---

<h1 class="text-2xl font-bold text-green-800 mb-4">Lessons</h1>

{% assign lessons_by_folder = site.pages | where_exp:"page","page.path contains 'lessons/' and page.path != 'lessons/lessonpage.md'" | group_by_exp:"page","page.path | split:'/' | slice:1,1 | first" %}

{% for folder in lessons_by_folder %}
  <h2 class="text-xl font-semibold text-green-700 mt-6 mb-2">{{ folder.name | capitalize }}</h2>
  <ul class="list-disc list-inside">
    {% for lesson in folder.items %}
      <li><a href="{{ lesson.url | relative_url }}" class="text-green-800 hover:text-green-600">{{ lesson.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

