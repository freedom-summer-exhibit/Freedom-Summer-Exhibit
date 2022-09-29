---
title: Resources
layout: default
image: /assets/images/Complete/Courage_04.jpg
image_alt: 
permalink: /resources
---
<div class="container-fluid">
  {% assign categories = site.education | sort: "page-order" %}
  <!-- Upper Row -->
    <div class="row">
    {% for card in categories %}
    {% if card.page-order < 5 %}
      <div class="col-6">
        <div class="card width-100 border-0 mb-2 bg-transparent">
        {% assign image_files = site.static_files | where: "image", true %}
        {% for myimage in image_files %}
        {% if myimage.basename == card.title %}
        <img src="/assets/images/Education/{{ myimage.name }}" class="card-img-top" alt="{{ myimage.basename }}" />
        {% endif %}
        {% endfor %}
          <div class="card-body">
            <h5 class="card-title">
              <a href="{{ card.url }}"> {{ card.title }}</a>
            </h5>
            <p class="card-text"> {{ card.size }} records</p>
          </div>
        </div>
      </div>
      {% endif %}
    {% endfor %}
    </div>
    </div>