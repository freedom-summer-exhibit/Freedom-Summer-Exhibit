---
title: Themes
layout: default
image: /assets/images/Complete/Empowerment_01_Replace.jpg
image_alt: Finding Freedom Summer Traveling Exhibit Themes Landing Page
permalink: /themes
---

## There are 12 themes designed to engage students to learn more.

<div class="row mt-5 d-flex justify-content-center" id="about_gallery">
{% assign theme_pages = site.themes %}
{% assign theme_items = site.data.image_captions %}
    {% for theme in theme_items %}
        {% if theme.Filename contains "1" %}
        <div class="card p-2 mt-3 border-0 bg-transparent col-12 col-sm-6 col-md-4 hv_container" style="max-width: 20rem">
        <a href="/themes/{{ theme.Themes | downcase }}">
            <img src="../assets/images/Complete/{{ theme.Filename }}" alt='{{ theme.Filename}}' class="card-img hv_image" />
            <div class="card-img-overlay hv_overlay">
            <h5 class="card-title text-white text-center hv_text">{{ theme.Themes }}</h5>
            </div>
        </a>
        </div>
        {% endif %}
    {% endfor %}
</div>