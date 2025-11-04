---
layout: default
title: "Tous les articles"
---

<nav style="margin-bottom: 2em; text-align: center;">
  <a href="{{ '/' | relative_url }}" style="margin: 0 10px;">Accueil</a> |
  <a href="{{ '/articles' | relative_url }}" style="margin: 0 10px;">Articles</a> |
  <a href="{{ '/about' | relative_url }}" style="margin: 0 10px;">À propos</a> 
</nav>

# Tous les articles

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})
*Publié le {{ post.date | date: "%d %B %Y" }}*

{{ post.excerpt | strip_html | truncate: 250 }}

[Lire la suite →]({{ post.url }})

---

{% endfor %}
