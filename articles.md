---
layout: default
title: "Tous les articles"
---

# Tous les articles

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})
*Publié le {{ post.date | date: "%d %B %Y" }}*

{{ post.excerpt | strip_html | truncate: 250 }}

[Lire la suite →]({{ post.url }})

---

{% endfor %}
