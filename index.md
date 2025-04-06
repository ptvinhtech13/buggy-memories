---
layout: home
title: Welcome
nav_order: 1
---

# Welcome to My Tech Journey 🚀🚀🚀

{: .highlight }
> "No Pain, No Gain" — unless you're using the right design patterns! 😉

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

## Who Am I? 🤔

Hello! I'm Vinh Pham (live in Ho Chi Minh City, Viet Nam), a software sorcerer with 9 years of experience in the tech industry. I have a passionate to build system from scratch, share knwoledge, and develop young colleage.

## Why This Blog? 💡

This is my digital garden where I cultivate and share:
- 🛠️ **Technical adventures**. Technical, Architecture, Culture, Coding Style, 
- Team development stories (featuring real humans!)
- Bug-hunting chronicles (some bugs are still at large)
- Conflict resolution tales (spoiler: git blame is not a conflict resolution tool)
- Mindset growth (because your brain needs updates too)

Let's make the software world a better place, one commit at a time! 🚀