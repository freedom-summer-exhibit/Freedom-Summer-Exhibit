---
title: Education Standards
layout: default
permalink: /education/education-standards
size: 3
page-order: 6
---

Lesson plans for the *Finding Freedom Summer Traveling Exhibit* were created to meet the following Ohio educational standards:


<ul class="list-unstyled">
    {% assign standards = site.data.related_resources | where: "category", "standard" %}
    {% for standard in standards %}
    <li class="mt-4 pb-2">
        <a href="{{ standard.url }}" target="_blank" class="h2"><i>{{ standard.linktext }}</i></a>
        {% if standard.linktext contains "Studies Standards" %}
        <p>Main 4th grade standards addressed in the lesson plans:</p>
            <div class="ps-5"><b>Historical Thinking and Skills</b>
            <p>2. Primary and secondary sources can be used to create historical narratives. (Page 18)</p>
            <p><b>Civic Participation and Skills</b><br />15. Individuals have a variety of opportunities to act in and influence their state and national government. Citizens have both rights and responsibilities in Ohio and the United States.<br />16. Civic participation in a democratic society requires individuals to make informed and reasoned decisions by accessing, evaluating and using information effectively to engage in compromise. (Page 19)</p>
            </div>
        {% else %}
        <p>{{ standard.description }}</p>
        {% endif %}
    </li>
    <hr>
    {% endfor %}
</ul>