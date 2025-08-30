---
layout: default
title: Home
---

## Latest Blog Posts
{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

---

## System Design Notes
{% assign notes = site.system_design | sort: "date" | reverse %}
{% for note in notes %}
- [{{ note.title }}]({{ note.url | relative_url }}) - {{ note.date | date: "%B %d, %Y" }}
{% endfor %}
