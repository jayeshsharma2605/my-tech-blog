---
layout: default
title: My Tech Blog
---

# Welcome to My Tech Blog

Explore articles on technology, tutorials, and system design concepts.

---

## Latest Blog Posts
<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a> 
    - <small>{{ post.date | date: "%B %d, %Y" }}</small>
  </li>
{% endfor %}
</ul>

---

## System Design Notes
<ul>
{% for note in site.system_design %}
  <li>
    <a href="{{ note.url }}">{{ note.title }}</a> 
    - <small>{{ note.date | date: "%B %d, %Y" }}</small>
  </li>
{% endfor %}
</ul>
