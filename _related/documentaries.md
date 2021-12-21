---
title: Documentaries
layout: default
permalink: /related/documentaries
size: 14
---

<ul>
    {% assign documentaries = site.data.related_resources | where: "category", "documentaries" %}
    {% for documentary in documentaries %}
    <li>
        <a href="{{ documentary.url }}" target="_blank">{{ documentary.title }}</a> {{ documentary.year }}
    </li>
    {% endfor %}
</ul>

<script>
    console.log("{{ documentaries | size }}");
</script>