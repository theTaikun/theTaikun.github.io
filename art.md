---
layout: page
title: Artwork
permalink: /art/
---


{% assign image_files = site.static_files | where: "art", true %}
{% for myimage in image_files %}
  <img src="{{ myimage.path }}" alt="{{myimage.name}}">
  {% endfor %}
