---
title: "Projects"
permalink: /projects/
layout: archive
---

# Projects

{% for project in site.projects %}
- **[{{ project.title }}]({{ project.url }})**  
  {{ project.description }}
{% endfor %}
