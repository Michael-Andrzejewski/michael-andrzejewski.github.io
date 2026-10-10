---
title: Soareverix Notes
---

Rough ideas and half-finished thinking by Michael Andrzejewski (Soareverix). Most of it is unpolished on purpose. Sections written by AI are labeled where they appear.

## Notes

{% assign notes = site.pages | where_exp: "p", "p.path contains 'ideas/'" | sort: "path" | reverse %}
{% for note in notes %}- [{{ note.title | default: note.name }}]({{ note.url | relative_url }}) <small>{{ note.path | remove: "ideas/" | slice: 0, 10 }}</small>
{% endfor %}
