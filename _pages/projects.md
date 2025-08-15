---
title: "Projects"
permalink: /projects/
layout: default
---

# Projects

{% for project in site.projects %}
- **[{{ project.title }}]({{ project.url }})**  
  {{ project.description }}
{% endfor %}
