---
layout: default
title: Education
permalink: "/education/"
comments: false
---
<!-- Home Intro
================================================== -->
{% if page.url == "/" %} 
<div class="rounded mb-5 hero">
  <div class="row align-items-center justify-content-between">
    <div class="col-md-6">
      <h1 class="font-weight-bold mb-4 serif-font">SCI-T</h1>
      <p class="lead mb-4">We drive progress through collaboration.</p>
      <a href="{{site.baseurl}}/about" class="btn btn-dark text-white px-5 btn-lg">About us</a>
    </div>
    <div class="col-md-6 text-right pl-0 pl-lg-4">
      <img class="intro" height="500" src="{{site.baseurl}}/assets/images/1.jpg">      
    </div>
  </div>
</div>
{% endif %}

<!-- Introduction to Education Section -->
<h1 class="font-weight-bold mb-4 serif-font">Welcome to the Education Section</h1>
<p class="lead mb-4">Explore resources, tips, and articles to enhance your learning journey.</p>

<!-- Posts List for Education Category -->
<section class="row">
  <div class="col-sm-8">
    <div class="row">
      {% for post in site.categories.education %}
        <div class="col-md-6 mb-5">
          {% include postbox.html %}
        </div>
      {% endfor %}
    </div>
  </div>

  <!-- Sidebar -->
  <div class="col-sm-4">
    {% include sidebar.html %}
  </div>
</section>

<!-- Pagination -->
<div class="bottompagination">
  <span class="navigation" role="navigation">
    {% include pagination.html %}
  </span>
</div>
