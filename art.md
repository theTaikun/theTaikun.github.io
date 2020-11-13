---
layout: page
title: Artwork
permalink: /art/
---


<iframe width="560" height="315" src="https://www.youtube.com/embed/WDTitMwt5mI" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


{% assign image_files = site.static_files | where: "art", true %}
{% for myimage in image_files %}
  <img src="{{ myimage.path }}" alt="{{myimage.name}}">
  {% endfor %}
