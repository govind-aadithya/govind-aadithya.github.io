---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

Publications
===
{% for post in site.publications reversed %}
  {% if post.categories == "publications" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

Patent
====
{% for post in site.publications reversed %}
    {% if site.collection == 'patent' %}
      {% include archive-single.html %}
    {% endif %}
{% endfor %}

