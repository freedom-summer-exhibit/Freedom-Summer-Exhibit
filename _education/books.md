---
title: Books and Documentaries
layout: default
permalink: /education/books-docs/
size: 30
page-order: 2
---

### Books

<ul>
    {% assign books = site.data.related_resources | where: "category", "books" %}
    {% for book in books %}
    <li>
        <a href="{{ book.url }}" target="_blank"><i>{{ book.title }}</i></a> by {{ book.author }}
    </li>
    {% endfor %}
</ul>

### Documentaries

<ul>
    {% assign documentaries = site.data.related_resources | where: "category", "documentaries" %}
    {% for documentary in documentaries %}
    <li>
        <a href="{{ documentary.url }}" target="_blank">{{ documentary.title }}</a> {{ documentary.year }}
    </li>
    {% endfor %}
</ul>

<script>
    console.log("{{ books | size }}");
    console.log("{{ documentaries | size }}");
</script>