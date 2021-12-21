---
title: Books
layout: default
permalink: /related/books/
size: 16
---

<ul>
    {% assign books = site.data.related_resources | where: "category", "books" %}
    {% for book in books %}
    <li>
        <a href="{{ book.url }}" target="_blank"><i>{{ book.title }}</i></a> by {{ book.author }}
    </li>
    {% endfor %}
</ul>

<script>
    console.log("{{ books | size }}");
</script>