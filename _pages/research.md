---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

You can also find my articles on <a href="https://scholar.google.com/citations?hl=en&user=fpjWEIUAAAAJ" style="color: rgb(255, 128, 0)">my Google Scholar profile<a> and the webpage of <u><a href="https://saferobotics.princeton.edu/research" style="color: rgb(255, 128, 0)">Safe Robotics Lab</a>.

{% include base_path %}

{% for post in site.research reversed%}
  {% include archive-single.html %}
{% endfor %}
