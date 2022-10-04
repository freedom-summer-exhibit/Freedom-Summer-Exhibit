---
title: Freedom Summer Lesson Plans
layout: default
permalink: /resources/lesson
size: 8
page-order: 4
---



<ul class="list-unstyled">
    {% assign lesson-plans = site.data.related_resources | where: "category", "lesson_plans" %}
    {% for lesson-plan in lesson-plans %}
    {% if forloop.index ==1 %}
    <h3>Lesson Plans for K-12</h3>
    <div class="mb-5">
    The following curriculum guides focus on the events of Freedom Summer and were designed to be used with digitized primary sources in the Freedom Summer Digital Collections supported by the Walter Havighurst Special Collections & University Archives at Miami University. Digitized material relating to Freedom Summer can be found in two digital collections: <a href="https://digital.lib.miamioh.edu/digital/collection/fstxt">The Freedom Summer Text & Photo Archive</a> and the <a href="https://digital.lib.miamioh.edu/digital/collection/fsavi">Freedom Summer AV Collection</a>. Original materials can be viewed in person at the Walter Havighurst Special Collections & University Archives at Miami University in Oxford, OH. 
    </div>
    {% elsif forloop.index == 9 %}
        <h3 class="my-5">Lesson Plans for Adults</h3>
    {% endif %}
    <li class="mt-4 pb-2">
    <a href="{{ lesson-plan.url }}" target="_blank" class="h3"><i>{{ lesson-plan.linktext }}</i></a>
        <p>Grade: {{ lesson-plan.grades }}</p>
        <p>{{ lesson-plan.description }}</p>
    </li>
    {% unless forloop.last %}
    <hr>
    {% endunless %}
    {% endfor %}
</ul>

