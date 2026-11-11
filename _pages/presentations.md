---
layout: archive
title: "Presentations and Posters"
permalink: /presentations/
author_profile: true
---

{% include base_path %}

{% assign presentation_list = site.presentations | sort: "date" | reverse %}

{% for post in presentation_list %}
  {% include archive-single-presentation.html %}
{% endfor %}
