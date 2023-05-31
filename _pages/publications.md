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


{% for work in site.collection.publications %}
  {% for post in site.publications reversed %}
        {% include archive-single.html %}
  {% endfor %}
{% endfor %}

Patent
====
{% for post in site.publications reversed %}
    {% if site.collection == 'patent' %}
      {% include archive-single.html %}
    {% endif %}
{% endfor %}
