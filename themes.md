---
title: Themes
layout: default
image: /assets/images/Complete/Empowerment_01_Replace.jpg
image_alt: "John Lewis, 1963. Photograph by Steve Schapiro. Portrait of John Lewis standing outside of a brick building in Clarksdale, Mississippi. Photograph in the collection of Miami University Art Museum, Oxford Ohio. Partial gift of the artist and partial purchase with contributions from the Kezur Endowment Fund (2019.23.12)."
permalink: /themes
---


<div class="mt-5 lead">Each panel in the exhibit has a big idea or theme relating to character traits of engaged citizenship, 2-4 photographs that relate to the big idea, and a historical narrative provided to add context for those who are engaging with the panels in more informal ways. The exhibit panel images presented here allow students to engage with powerful visual imagery and storytelling  and can be used as a supplement to the lesson plans or exhibit panel viewing.</div>

<div class="row mt-5 d-flex justify-content-center" id="about_gallery">
{% assign theme_items = site.data.image_captions %}
    {% for theme in theme_items %}
        {% if theme.Filename contains "1" %}
        <div class="card p-2 mt-3 border-0 bg-transparent col-12 col-sm-6 col-md-4 hv_container" style="max-width: 20rem">
        <a href="/themes/{{ theme.Themes | downcase }}">
            <img src="../assets/images/Complete/{{ theme.Filename }}" alt='{{ theme.CreditLine | escape }}' class="card-img hv_image" />
            <div class="card-img-overlay hv_overlay">
            <h5 class="card-title text-white text-center hv_text">{{ theme.Themes }}</h5>
            </div>
        </a>
        </div>
        {% endif %}
    {% endfor %}
</div>