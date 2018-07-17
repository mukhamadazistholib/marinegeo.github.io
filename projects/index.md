---
layout: default
title: Projects
use-site-title: true
---


{% assign sorted = site.projects | sort: "weight" %}
{% for cat in sorted %}

<div class="col-md-12 col-md-offset-1" style="width: 200px; padding-top: 25px;">
 <a href="{{site.baseurl}}{{cat.url}}">
   <img src="{{ cat.thumbnail }}" class="img-responsive" style="height: 150px; position: relative; left: 50%; top: 50%; margin-left: -75px;">
  <h4 style="text-align:center">{{cat.title}}</h4>
</a>
</div>
{% endfor %}
