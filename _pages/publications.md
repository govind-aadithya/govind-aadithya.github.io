---
layout: archive
title: 
permalink: /research/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

Patent
====

{% for post in site.publications %}
  {% for tag in post.tags %}
    {% if tag == "patent" %}
      {% include archive-single.html %}      
    {% endif %}
  {% endfor %}
{% endfor %}


Publications
===

{% for post in site.publications %}
  {% for tag in post.tags %}
    {% if tag == "publications" %}
      {% include archive-single.html %}      
    {% endif %}
  {% endfor %}
{% endfor %}


Thesis
===

{% for post in site.publications %}
  {% for tag in post.tags %}
    {% if tag == "thesis" %}
      {% include archive-single.html %}      
    {% endif %}
  {% endfor %}
{% endfor %}

Unpublished Works
===

{% for post in site.publications %}
  {% for tag in post.tags %}
    {% if tag == "unpublished" %}
      {% include archive_single_unpub.html %}      
    {% endif %}
  {% endfor %}
{% endfor %}
