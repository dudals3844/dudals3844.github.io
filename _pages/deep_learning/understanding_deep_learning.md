---
title: "Deep Learning/Understanding Deep Learning"
layout: category
permalink: /deep_learning/understanding_deep_learning
author_profile: true
sidebar_main: true
types: posts
taxonomy:
    category:
        - understanding_deep_learning
sidebar:
  nav: "sidebar-category"
  enabled: true
---

{% assign main_category = site.posts | where: "categories", "deep_learning" %}
{% assign sub_category = main_category | where: "categories", "understanding_deep_learning" %}

{% for post in sub_category %}
  {% include archive-single.html type=page.entries_layout %}
{% endfor %}
