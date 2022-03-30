---
title: Freedom Summer at Miami University
layout: default
permalink: /resources/fsmu
size: 7
---

<ul>
    {% assign activities = site.data.related_resources | where: "category", "activities"%}
    {% for activity in activities %}
    <li>
        <a href="{{ activity.url }}" target="_blank">{{ activity.title }}</a>
    </li>
    {% endfor %}
</ul>

<script>
    console.log("{{ activities | size }}");
</script>