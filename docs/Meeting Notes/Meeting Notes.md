---
title: "Meeting Notes"
layout: default
nav_order: 0
---

{% assign notes = site.pages | where: "parent", "Meeting Notes" | sort: "date" | reverse %}
{% for note in notes %}
- [{{ note.title }}]({{ note.url }})
{% endfor %}