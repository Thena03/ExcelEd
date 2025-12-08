---
layout: base
title: Lessons
---

<h1 class="text-3xl font-bold text-green-800 mb-6">Lessons</h1>

{% comment %}
Filter out the current index page and select all pages in the lessons folder
{% endcomment %}
{% assign lesson_pages = site.pages | where_exp:"page","page.path contains 'lessons/' and page.path != 'lessons/index.md'" %}

{% comment %}
Group the lessons by the first folder after 'lessons/'
{% endcomment %}
{% assign lessons_by_folder = lesson_pages | group_by_exp:"page","page.path | split: '/' | slice:1,1 | first" %}

<div class="space-y-8">
  {% for folder in lessons_by_folder %}
    <div>
      <h2 class="text-2xl font-semibold text-green-700 mb-2">{{ folder.name | capitalize }}</h2>
      <ul class="list-disc list-inside space-y-1">
        {% for lesson in folder.items %}
          <li>
            <a href="{{ lesson.url | relative_url }}" class="text-green-800 hover:text-green-600">{{ lesson.title }}</a>
          </li>
        {% endfor %}
      </ul>
    </div>
  {% endfor %}
</div>
