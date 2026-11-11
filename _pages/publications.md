---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

## First-Author Publications

{% assign first_author_papers = site.publications | sort: "date" | reverse %}

{% for post in first_author_papers %}
  {% if post.author_position == "first" %}
    {% include archive-single-publication.html %}
  {% endif %}
{% endfor %}

## Co-Authored Publications

{% assign coauthored_papers = site.publications | sort: "date" | reverse %}

{% for post in coauthored_papers %}
  {% if post.author_position == "coauthor" %}
    {% include archive-single-publication.html %}
  {% endif %}
{% endfor %}
