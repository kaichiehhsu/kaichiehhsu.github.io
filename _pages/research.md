---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

You can also find my articles on <u><a href="https://scholar.google.com/citations?hl=en&user=fpjWEIUAAAAJ">my Google Scholar profile<a>.

{% include base_path %}

<h2 style="color:#ff8000">
  Ongoing Projects
</h2>
{% for post in site.ongoing %}
  {% include archive-single.html %}
{% endfor %}

<h2 style="color:#ff8000">
  Selected Completed Projects
</h2>
{% for post in site.research reversed %}
  {% include archive-single.html %}
{% endfor %}