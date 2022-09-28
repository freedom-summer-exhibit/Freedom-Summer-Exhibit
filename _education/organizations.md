---
title: Organizations and Archives
layout: default
permalink: /education/organizations/
size: 12
page-order: 5
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