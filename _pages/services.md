---
layout: single  # Use the layout you prefer
title: "Services"
permalink: /services/ 
---

## Reviews
{% for review in site.reviews %}
### {{ review.title }}
**Date:** {{ review.date }}  
**Description:** {{ review.description }}  

{{ review.content }}
{% endfor %}

## Volunteering
{% for volunteering in site.volunteering %}
### {{ volunteering.title }}
**Date:** {{ volunteering.date }}  
**Description:** {{ volunteering.description }}  

{{ volunteering.content }}
{% endfor %}
