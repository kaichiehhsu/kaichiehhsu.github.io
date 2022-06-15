---
layout: archive
title: "Past Projects"
permalink: /past_projects/
author_profile: true
---

{% include base_path %}

{% for post in site.past_projects reversed %}
  {% include archive-single.html %}
{% endfor %}