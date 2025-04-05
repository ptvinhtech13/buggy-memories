---
layout: home
title: Home
nav_order: 1
---

# Welcome to My Tech Journey

{: .highlight }
> Software Engineer documenting solutions, learnings, and occasional bugs.

## Recent Updates
{% assign recent_posts = site.pages | where_exp:"page", "page.parent == 'Tech Journey'" | sort: "date" | reverse | limit: 5 %}

<div class="recent-posts">
{% for post in recent_posts %}
  <div class="post-card">
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
    {% if post.description %}
    <p>{{ post.description }}</p>
    {% endif %}
  </div>
{% endfor %}
</div>