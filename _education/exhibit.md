---
title: Exhibit Lesson Plans
layout: default
permalink: /education/exhibit-lesson-plans
size: 12
page-order: 5
---

Lesson plans for Ohio 4th and 5th grade students were created by ART 195 – Introduction to Art Education Miami University students in Spring 2021. The following lesson plans can be used independently or in conjunction with a viewing of the *Finding Freedom Summer Traveling Exhibit.*

<ul class="list-unstyled">
    {% assign exhibits = site.data.related_resources | where: "category", "exhibit" %}
    {% for exhibit in exhibits %}
    <li class="mt-4 pb-2">
    <h3><small>{{ exhibit.title }}</small></h3>
        <a href="{{ exhibit.url }}" target="_blank" class="h2"><i>{{ exhibit.linktext }}</i></a>
        <p>Grade: {{ exhibit.grades }}</p>
        <p>{{ exhibit.description }}</p>
    </li>
    {% unless forloop.last %}
    <hr>
    {% endunless %}
    {% endfor %}
</ul>