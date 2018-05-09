---
title: "Projects"
layout: single
permalink: "/projects/"
header:
  overlay_image: /assets/images/projects/projects.png
  overlay_filter: 0.6 # same as adding an opacity of 0.5 to a black background
author_profile: true
---

Over the years, we have been able to venture into quite a variety of projects-topics. We present a few of them here.

You may click on the subheadings to view the entire list.

## [Projects](/projects)
{% for item in site.projects %}
  {% if forloop.index==6 %}
  {% break %} // won't work
  {% endif %}
  <h3><a href="{{ item.url }}">{{ item.title }}</a></h3>
  <p>{{ item.description }}</p>
{% endfor %}
