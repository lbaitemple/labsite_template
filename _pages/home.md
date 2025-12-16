---
title: "Home"
layout: homelay
excerpt: "Your Lab at Your University"
sitemap: false
permalink: /
---

## Welcome to [Your Lab Name]

We are a research group at [Your University] focused on [your research areas].

Our mission is to advance the state of the art in [your field] through innovative research and collaboration.

[Learn more about our research]({{ site.baseurl }}/research){: .btn .btn-primary .btn-lg}

<div class="row" style="margin-top: 30px;">
  <div class="col-sm-8" markdown="1">

## About the Lab

Welcome to [Your Lab Name]. We are a research group at [Your University] focused on [your research areas].

Our research interests include:
- Research area 1
- Research area 2
- Research area 3
- Research area 4

We collaborate with industry partners and academic institutions worldwide to advance the state of the art in [your field].

### Research Focus

Our work addresses fundamental challenges in:
- Challenge area 1
- Challenge area 2
- Challenge area 3

We develop innovative solutions that combine theory and practice to solve real-world problems.

  </div>
  
  <div class="col-sm-4" markdown="1">

## News & Updates

<div class="panel panel-default">
  <div class="panel-body">
    <h4>Latest News</h4>
    <ul class="list-unstyled">
      {% for news in site.data.news limit:5 %}
      <li style="margin-bottom: 15px;">
        <strong>{{ news.date }}</strong><br>
        {{ news.headline }}
      </li>
      {% endfor %}
    </ul>
    <a href="{{ site.baseurl }}/news" class="btn btn-sm btn-default">View all news</a>
  </div>
</div>

### Quick Links

<div class="list-group">
  <a href="{{ site.baseurl }}/team" class="list-group-item">
    <span class="glyphicon glyphicon-user"></span> Meet Our Team
  </a>
  <a href="{{ site.baseurl }}/publications" class="list-group-item">
    <span class="glyphicon glyphicon-book"></span> Publications
  </a>
  <a href="{{ site.baseurl }}/software" class="list-group-item">
    <span class="glyphicon glyphicon-download-alt"></span> Software & Tools
  </a>
  <a href="{{ site.baseurl }}/openings" class="list-group-item">
    <span class="glyphicon glyphicon-briefcase"></span> Join Us
  </a>
</div>

  </div>
</div>
