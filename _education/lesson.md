---
title: Freedom Summer Lesson Plans
layout: default
permalink: /resources/lesson
size: 8
page-order: 4
---

<ul>
    {% assign booksByAge = site.data.related_resources | where: "category", "lesson_plans" %}
    {% for book in booksByAge %}
    <li>
        <a href="{{ book.url }}" target="_blank"><i>{{ book.title }}</i></a> by {{ book.author }}{% if book.illustrator%}, Illustrated by {{ book.illustrator }}{% endif %}
        <p>Ages: {{book.ages}}</p>
        <p>Desciption: {{book.description}}</p>
    </li>
    {% endfor %}
</ul>

