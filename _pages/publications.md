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
    {% include archive-single.html %}
{% endfor %}


Patent
====

{% for tag in site.publications.tags %}
  <h2>{{ tag }}</h2>
  {% for post in tag %}
    {% include archive-single.html %}      
  {% endfor %}
{% endfor %}

<!--{% for post in site.publications %}
    {% if post.tags == "patent" %}
      {% include archive-single.html %}
    {% endif %}
{% endfor %}-->
