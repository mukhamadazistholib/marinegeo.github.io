---
layout: pagelink2edit
title: MarineGEO Data
subtitle: Data Standards and Guidelines
use-site-title: true
---

## Purpose

Collaborative website for people in the MarineGEO network to discover methods, learn data management techniques, and download methods and data entry templates.

## Project Modules

Project modules are packages that contain instructions for deploying experiments, data entry templates and field sheets.

{% assign sorted = site.project-modules | sort: "weight" | where_exp:"item", "item.submodule != true" %}

{% for project-module in sorted %}
<div class="col-md-3 col-sm-4 col-xs-6">
  <div style="padding-top: 25px;">
 <a href="{{site.baseurl}}{{project-module.url}}">
   <img src="{{ project-module.thumbnail }}" class="img-responsive" style="height: 150px; position: relative; left: 50%; top: 50%; margin-left: -75px;">
  <h4 style="text-align:center">{{project-module.title}}</h4>
</a>
</div>
</div>
{% endfor %}
