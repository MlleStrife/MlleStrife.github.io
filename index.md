---
layout: home
title: "Bienvenue sur mon espace de réflexion et de formation en cybersécurité"
description: "Réflexions sur l'informatique, analyses et retours d’expérience autour de l’intelligence artificielle  & formation en cybersécurité. Bienvenue sur ma home page."
---


<nav style="margin-bottom: 2em; text-align: center;">
  <a href="{{ '/' | relative_url }}" style="margin: 0 10px;">Accueil</a> |
  <a href="{{ '/articles' | relative_url }}" style="margin: 0 10px;">Articles</a> |
  <a href="{{ '/about' | relative_url }}" style="margin: 0 10px;">À propos</a> 
</nav>

# Bonjour !

Moi c'est Manon, et ici je vais parler de mes passions. L'enseignement et la formation sont mes moteurs : pour moi, la connaissance et le savoir doit être partagé. J'ai longtemps fait des vacations à l'université dans les domaines de l'informatique suite à mon doctorat dans l'IA (plus précisément le traitement de la parole et des émotions). Depuis quelques mois, je me suis tournée vers le monde de la cybersécurité, un domaine passionnant qui est essentiel dans nos vies.

Je partage ici mes réflexions, mes trouvailles et je propose des formations axées sur la cybersécurité.  
Si tu t’intéresses à la **cybersécurité** dans son ensemble ou dans ses détails, tu es au bon endroit.

---

## Derniers articles

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url }})
*Publié le {{ post.date | date: "%d %B %Y" }}*

{{ post.excerpt | strip_html | truncate: 200 }}

[Lire la suite →]({{ post.url }})

---

{% endfor %}

---

## Les prochains articles prévus

### Le phising : formation complète
Quand on pense cybersécurité, on finit par penser au phising. Cette porte d'entrée, souvent mal gardée (manque de formation, de vigilance, attaque de plus en plus sophostiquée...), peut mener à des conséquences désastreuses. [to be continued]
Date de sortie : 15/11/2025

 ---

### L'IA hybride appliqué à la cybersécurité
L’intelligence artificielle hybride, croisement entre approche symbolique et apprentissage automatique, s’impose comme une réponse concrète aux défis de la cybersécurité d'aujourd'hui. Entre explicabilité et performance, elle redéfinit la manière dont les SOC anticipent, détectent et réagissent aux menaces. [to be continued]
Date de sortie : 01/12/2025