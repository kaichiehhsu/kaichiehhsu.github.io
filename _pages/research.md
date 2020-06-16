---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

You can also find my articles on <u><a href="https://scholar.google.com/citations?hl=en&user=fpjWEIUAAAAJ">my Google Scholar profile<a>.

{% include base_path %}

{% for post in site.research %}
  {% include archive-single.html %}
{% endfor %}
