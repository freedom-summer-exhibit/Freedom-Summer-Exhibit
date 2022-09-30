---
title: Education Standards
layout: default
permalink: /education/education-standards
size: 5
page-order: 6
---

Lesson plans for the *Finding Freedom Summer Traveling Exhibit* were created to meet the following Ohio educational standards:


<ul class="list-unstyled">
    {% assign standards = site.data.related_resources | where: "category", "standard" %}
    {% for standard in standards %}
    <li class="mt-4 pb-2">
        <a href="{{ standard.url }}" target="_blank" class="h2"><i>{{ standard.linktext }}</i></a>
        <p>Grade: {{ standard.grades }}</p>
        <p>{{ standard.description }}</p>
    </li>
    <hr>
    {% endfor %}
</ul>