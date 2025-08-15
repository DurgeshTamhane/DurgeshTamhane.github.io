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


---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}


{% for post in site.projects %}
  {% include archive-single.html %}
{% endfor %}
