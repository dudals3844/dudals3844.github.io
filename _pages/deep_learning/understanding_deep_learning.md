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

{% assign deep_learning_post = site.posts | where: "categories", "deep_learning" %}
{% assign deep_learning_post_with_understanding = deep_learning_post | where: "categories", "understanding_deep_learning" %}

{% for post in deep_learning_post_with_understanding %}
  {% include archive-single.html type=page.entries_layout %}
{% endfor %}
