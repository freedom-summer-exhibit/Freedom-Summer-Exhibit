---
title: Related Resources
layout: default
image: /assets/images/Untitled_7.jpeg
image_alt: Related Resources
permalink: /related/
---
## Related Resources 

The Freedom Summer Traveling exhibit connects a powerful
chapter of U.S. civil rights history to current day challenges, “Finding Freedom
Summer” offers timely reminders of our nation’s troubled history, emphasizes the
social-emotional attributes of those who stand to make a difference, and
challenges youth to find and understand the power of their voices. Designed for
students in the fourth grade level, the exhibit focuses on the summer of 1964
and the Freedom Summer training that took place on Oxford, Ohio’s, Western
College for Women, this deep learning project, rooted in art integration but
versatile in its applications, challenges students to apply four active learning
capacities.

<div class="container-fluid">
  {% assign categories = site.related %}
  <!-- Upper Row -->
    <div class="row">
    {% for card in categories %}
      {% if forloop.index < 3 %} 
      <div class="col">
        <div class="card width-100 border-0 mb-2 bg-transparent">
          <img src="/assets/images/placeholder.png" class="card-img-top" alt="..." />
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
    <!-- Lower Row -->
    <div class="row">
    {% for card in categories %}
      {% if forloop.index >= 3 %} 
      <div class="col">
        <div class="card width-100 border-0 mb-2 bg-transparent">
          <img src="/assets/images/placeholder.png" class="card-img-top" alt="..." />
          <div class="card-body">
            <h5 class="card-title">
              <a href="{{ card.url }}"> {{ card.title }}</a>
            </h5>
            <p class="card-text"> {{ card.size }} of records</p>
          </div>
        </div>
      </div>
    {% endif %}
    {% endfor %}
    </div>

</div>

<div class="container --bs-bg-opacity" style="padding-top: 2rem">
  <div class="col-md-12 text-center">
    <button type="button" class="btn btn-dark">View All Resources</button>
  </div>
</div>