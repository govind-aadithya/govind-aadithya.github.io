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
  {% capture filename %}
    {% if filename <> 'patent' or filename <> 'Patent' %}
        {% include archive-single.html %}
    {% endif %}
  {% endcapture %} 
{% endfor %}

Patent
====
{% for post in site.publications reversed %}
  {% capture filename %}
    {% if filename == 'patent' or filename == 'Patent' %}
      {% include archive-single.html %}
    {% endif %}
  {% endcapture %}
{% endfor %}
