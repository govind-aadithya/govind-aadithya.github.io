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

{% for post in site.publications reversed %}
    {% if site.collection <> 'patent' or site.collection <> 'Patent' %}
        {% include archive-single.html %}
    {% endif %}
{% endfor %}

Patent
====
{% for post in site.publications reversed %}
    {% if site.collection == 'patent' or site.collection == 'Patent' %}
      {% include archive-single.html %}
    {% endif %}
{% endfor %}
