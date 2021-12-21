---
title: Books for Children, Teens, & Young Adults
layout: default
permalink: /related/books-by-age
size: 8
---

<ul>
    {% assign booksByAge = site.data.related_resources | where: "category", "books_by_age" %}
    {% for book in booksByAge %}
    <li>
        <a href="{{ book.url }}" target="_blank"><i>{{ book.title }}</i></a> by {{ book.author }}{% if book.illustrator%}, Illustrated by {{ book.illustrator }}{% endif %}
        <p>Ages: {{book.ages}}</p>
        <p>Desciption: {{book.description}}</p>
    </li>
    {% endfor %}
</ul>

<script>
    console.log("{{ booksByAge | size }}");
</script>

