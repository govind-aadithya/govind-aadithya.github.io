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

{% for category in site.categories %}
    {% capture category_name %}{{ category | first }}{% endcapture %}
    {% for post in site.categories[category_name] %}
      {% include archive-single.html %}
    {% endfor %}
{% endfor %}

<!--
{% for category in site.categories %}
  {% for post in work.publications reversed %}
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
-->
