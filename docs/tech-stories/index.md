---
layout: default
title: Technical Story
nav_order: 2
has_children: true
permalink: /tech-story
---

# Tech Stories

Welcome to my technical documentation collection. Here you'll find detailed solutions, learnings, and experiences from my software engineering journey.

## Latest Solutions

{% assign solutions = site.pages | where_exp:"page", "page.parent == 'Tech Journey'" | sort: "date" | reverse %}
{% for solution in solutions %}
{% if solution.title != page.title %}
- [{{ solution.title }}]({{ solution.url | relative_url }}) - {{ solution.description }}
{% endif %}
{% endfor %}
