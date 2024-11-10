---
layout: single  # Use the layout you prefer
title: "Supervision"
permalink: /supervision/ 
---
## Supervision
{% assign sorted_super = site.supervision | sort: "date" | reverse %}
{% for super in sorted_super %}
- **{{ super.title }}**
  **Period:** From {{ super.date | date: "%Y-%m"}} To  {{ super.dateend | date: "%Y-%m"}}
  {% if super.many==true %}
  **Students:** {{ super.students}}
  {% else %}
  **Student:** {{ super.students}}
  {% endif %}
{% endfor %}