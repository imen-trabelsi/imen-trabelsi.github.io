---
layout: single  # Use the layout you prefer
title: "Services"
permalink: /services/ 
---

## Reviews
{% assign sorted_reviews = site.reviews | sort: "date" | reverse %}
{% for review in sorted_reviews %}
### {{ review.title }}
**Venue:** {{ organization.venue }}  
**Date:** {{ review.date | date: "%Y-%m"}}  

{% endfor %}

## Volunteering
{% assign sorted_organization= site.organization | sort: "date" | reverse %}
{% for organization in sorted_organization %}
### {{ organization.title }}
**Event:** {{ organization.event }}  
**Date:** {{ organization.date | date: "%Y-%m-%d"}}  
**Description:** {{ organization.description }}  
{% endfor %}
