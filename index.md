---
layout: page
title: MarineGEO Data
subtitle: Data Standards and Guidelines
use-site-title: true
editbutton: false
modules:
  - /modules/seagrass
  - /modules/benthicphotos
  - /modules/squidpops
  - /modules/waterquality
  - /modules/panamex-photoquadrat-scoring
  - /modules/uav
---

## Purpose

Collaborative website for people in the MarineGEO network to discover methods, learn data management techniques, and download methods and data entry templates.

## Project Modules

Project modules are packages that contain instructions for deploying experiments, data entry templates and field sheets.

{% assign sorted = site.project-modules | sort: 'title' %}

{% if page.modules %}
  {% for m in page.modules %}
  {% for module in sorted %}
    {% if m == module.id  %}
<div class="col-md-3 col-sm-4 col-xs-6" style="height: 225px;">
  <a href="{{site.baseurl}}{{module.url}}">
         <img src="{{module.thumbnail}}" class="img-responsive" style="height: 150px; position: relative; left: 50%; top: 50%; margin-left: -75px;">
        <h4 style="text-align:center">{{module.title}}</h4>
      </a>
</div>
    {% endif %}
  {% endfor %}
  {% endfor %}
{% endif %}
