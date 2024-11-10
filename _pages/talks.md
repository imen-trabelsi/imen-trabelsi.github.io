---
layout: single  # Use the layout you prefer
title: "Talks"
permalink: /talks/ 
---

## Talks
{% assign sorted_talks = site.talks | sort: "date" | reverse %}
{% for talk in sorted_talks %}
- ### {{ talk.title }}
**Venue:** {{ talk.venue }}  
**Date:** {{ talk.date | date: "%Y-%m-%d"}}  
 {{ talk.discription}}  
{% endfor %}