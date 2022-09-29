---
title: Education
layout: default
image: /assets/images/Complete/Passion_03_New.jpg
image_alt: Education
permalink: /education
---

## {{page.title}}

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

<div class="container col bg-secondary bg-opacity-25">
    <!-- Upper Row -->
    <div class="row" style="margin-top: 2rem;">
        <div class="col">
            <!-- Card 1 -->
            <div class="card width-100 border-0 mb-2 bg-transparent">
                <div class="card-body">
                    <!-- Cannot currently see if this will appear as we want-->
                    <div class="float-start">
                        <img src="/assets/images/Icons/Recognize_icon.png" alt="Recognize" class="circle">
                    </div>
                    <h5 class="card-title" style="margin-left: 4rem;">Recognize</h5>
                    <p class="card-text" style="margin-left: 4rem;">connections between Freedom Summer's people, places, and topics through visual communication and scaffolded reflection.</p>
                </div>
            </div>
        </div>
        <div class="col">
            <!-- Card 2 -->
            <div class="card width-100 border-0 mb-2 bg-transparent">
                <div class="card-body">
                    <!-- Cannot currently see if this will appear as we want-->
                    <div class="float-start">
                        <img src="/assets/images/Icons/Create_icon.png" alt="Create" class="circle">
                    </div>
                    <h5 class="card-title" style="margin-left: 4rem;">Create</h5>
                    <p class="card-text" style="margin-left: 4rem;">a visual representation communicating new understanding of Freedom Summer, relating a big idea connecting the past, present, and personal experience.</p>
                </div>
            </div>
        </div>
    </div>
    <!-- Under Row -->
    <!-- Card 3 -->
    <div class="row" style="margin-bottom: 3rem;">
        <div class="col">
            <div class="card width-100 border-0 mb-2 bg-transparent">
                <div class="card-body">
                    <div class="float-start">
                        <img src="/assets/images/Icons/Synthesize_icon.png" alt="Synthesize" class="circle">
                    </div>
                    <h5 class="card-title" style="margin-left: 4rem;">Synthesize</h5>
                    <p class="card-text" style="margin-left: 4rem;">historical content with personal experiences to increase empathy for others and advocate for human rights and social justice.</p>
                </div>
            </div>
        </div>
        <!-- Card 4 -->
        <div class="col">
            <div class="card width-100 border-0 mb-2 bg-transparent">
                <div class="card-body">
                    <div class="float-start">
                        <img src="/assets/images/Icons/Reflect_icon.png" alt="Reflect" class="circle">
                    </div>
                    <h5 class="card-title" style="margin-left: 4rem;">Reflect</h5>
                    <p class="card-text" style="margin-left: 4rem;">on meaning through artwork, individually and collectively, privately and in public spaces educating others in the community.</p>
                </div>
            </div>
        </div>
    </div>
</div>

<div class="container-fluid">
  {% assign categories = site.education | sort: "page-order" %}
  <!-- Upper Row -->
    <div class="row">
    {% for card in categories %}
    {% if card.page-order >= 5 %}
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

<div class="container --bs-bg-opacity mt-4">
  <div class="col-md-12 text-center">
    <button type="button" class="btn btn-dark">Download All Lesson Plans</button>
  </div>
</div>
