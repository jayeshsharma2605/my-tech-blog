---
layout: default
title: My Tech Blog
---

# Welcome to My Tech Blog

Explore articles on technology, tutorials, and system design concepts.

---

## Latest Blog Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

---

## System Design Notes

{% for note in site.system_design %}
- [{{ note.title }}]({{ note.url }}) - {{ note.date | date: "%B %d, %Y" }}
{% endfor %}
