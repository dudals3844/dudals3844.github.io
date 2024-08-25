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

{% assign posts_with_deep_learning = site.posts | where: "categories", "deep_learning" %}
{% assign posts_with_deep_learning_and_books = posts_with_deep_learning | where: "categories", "understanding_deep_learning" %}

{% for post in posts_with_deep_learning_and_books%}
  {% include archive-single.html type=page.entries_layout %}
{% endfor %}
