---
title: Organizations and Archives
layout: default
permalink: /resources/organizations/
size: 12
---

<ul>
    {% assign organizations = site.data.related_resources | where: "category", "organizations" %}
    {% for organization in organizations %}
    <li>
        <a href="{{ organization.url }}" target="_blank">{{ organization.title }}</a>
    </li>
    {% endfor %}
</ul>

<script>
    console.log("{{ organizations | size }}");
</script>