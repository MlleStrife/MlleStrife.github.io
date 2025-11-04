---
layout: post
title: "Pourquoi tout n’est pas \"GenIA\"l dans l’intelligence artificielle — et quelles sont les alternatives ?"
date: 2025-09-01
author: "MlleStrife"
description: "L’IA générative fascine, mais elle n’est qu’une toute petite partie de l’intelligence artificielle. Aujourd'hui les masses semblent les rendre indissociables. Petit tour d’horizon des alternatives plus sobres, plus explicables et souvent plus pertinentes."
tags: [IA, Intelligence Artificielle, Machine Learning, GenIA, Éthique]
---

> Aujourd'hui tout le monde parle d’intelligence artificielle, mais soyons honnêtes : quand on dit “IA”, on pense surtout à ChatGPT et toutes ses variantes.  
> Sauf que tout n’est pas “GenIA”l, et surtout… tout ne devrait pas l’être.

---

## Pourquoi tout n’est pas "GenIA"l dans l’intelligence artificielle? Et quelles sont les alternatives ?

Fin 2022, OpenAI dépose dans les mains de milliers d’utilisateurs curieux sa création : **ChatGPT**.  
En quelques mois à peine, les utilisateurs se multiplient et se diversifient, atteignant environ **30 millions** en janvier 2023 ([source : NBER Working Paper, 2024](https://www.nber.org/papers/w34255)). 
Ce nombre colossal d'utilisateurs est d'abord composé de connaisseurs en IA et en informatique. Ces derniers laissent leur place à une écrasante majorité de tout un chacun pour atteindre aujourd'hui en fin 2025 les **700 millions d'utilisateurs** chaque semaine ([source : OpenAI](https://openai.com/index/how-people-are-using-chatgpt/)]. Ce sont des nombres qui donnent le vertige, qu'en pensez vous ?

Pour mieux comprendre ces chiffres, il suffit de comparer avec d’autres services du web qui peuplent Internet.  
Un petit graphique (celui d’[EconomyApp sur X](https://x.com/EconomyApp/status/1622029832099082241) par exemple) montre que ChatGPT a connu une **adoption plus rapide qu’Instagram, TikTok ou Netflix**.  Bref, un vrai raz-de-marée numérique.  


Face à cette explosion, le mot **“IA”** (Intelligence Artificielle) est devenu presque synonyme de **“GenIA”** (IA générative).  
Texte, image, code, musique, vidéo : la “GenIA” fascine par ses capacités créatives et son apparente poluvalence. 
Mais derrière tout cet engouement médiatique et financier, une réalité plus nuancée se cache : **tout n’est pas GenIA dans l’IA.**  
Et surtout, **tout ne doit pas l’être.**

---

## 1. La GenIA : une révolution… surtout dans son accessibilité

L’IA générative repose sur des modèles de très grande taille (*Large Language Models* — le nom est déjà un indice) entraînés sur d’immenses quantités de données.
Ces modèles apprennent à **reproduire la forme** de nos productions : rédiger, dialoguer, illustrer. Mais pas forcément à comprendre le fond.
Leur puissance vient du volume colossal de données utilisées pour leur apprentissage, de leur architecture complexe (le fameux *Transformer*) et de leurs milliards de paramètres.

Si vous voulez creuser, tout part de la publication **[Attention is all you need](https://arxiv.org/abs/1706.03762)** (Vaswani et al., 2017).  
Et pour une explication claire et accessible, le [cours LLM de Hugging Face](https://huggingface.co/learn/llm-course/fr/chapter1/4) est une super ressource.

Mais la **vraie révolution** a consisté à sortir un outil des laboratoires de recherche et à le mettre dans **les mains de tous**, avec une interface simple : tout le monde sait discuter, tout le monde peut donc l'essayer.  
Cette accessibilité lui a permis de se faire une place de choix dans la vie et la tête de bon nombre de personne pour qui l'IA était un concept abstrait auparavant. 
ChatGPT et ses futures déclinaisons ont alors revêtit la définition même de l'IA pour le grand nombre, ce qui a impacté les chercheurs du monde entier et les a incité à s'engouffrer dans cet axe de recherche. Mais en vérité, la GenIA, ce n’est qu’un **petit morceau du grand puzzle de l’IA**.

---

## 2. L’IA, un domaine bien plus large

Bien avant l’arrivée de ChatGPT, l’intelligence artificielle existait déjà sous de nombreuses formes. Les chercheurs et ingénieurs utilisaient — et utilisent encore — des approches variées, souvent bien plus adaptées à des contextes précis.

### - L’IA symbolique  
C’est l’approche “old school” : on programme des **règles logiques** pour résoudre des problèmes. 
Un exemple simple : la coorection de la grammaire. Si le sujet est “je”, alors le verbe qui suit est à la première personne du singulier.  
Tout est explicable, tout est rationnel.  
Le seul problème, c’est qu’il faut penser à tous les cas possibles (et là, bon courage).

### - Le machine learning "classique"  
Avant les réseaux neuronaux profonds (Deep Learning), le *machine learning* utilisait des modèles plus compacts : régression logistique, arbres de décision, SVM, k-means… Ces derniers fonctionnent selon des algorithmes mathématiques et donnent **des systèmes déterministes** (la même entrée donne la même sortie), consomment **peu de ressources**, et sont souvent **plus faciles à expliquer**.  
Un exemple simple : un lecteur de chiffre manuscrit. Je donne une image d'un huit, le système me dit que c'est un huit (un peu comme les captchas de l'époque).
Ils sont encore hyper présents aujourd’hui : détection de fraude, maintenance prédictive, scoring de risque, reconnaissance de caractères…  
Bref, du concret, fiable, efficace.

### - L’IA hybride  
Entre les deux mondes, on trouve l’**IA hybride** (ou **neurosymbolique**).  
L’idée : combiner logique et apprentissage automatique.  
Résultat : des modèles à la fois performants et explicables ce qui est parfait pour des domaines où on ne peut pas se permettre l’erreur (santé, justice, cybersécurité notamment).  
C’est un sujet de recherche très actif (voir le [NeSy Workshop](https://2025.nesyconf.org/)). Un article plus détaillé sera consacré à l'IA hybride appliqué à la cybersécurité dans les prochaines semaines.

---

## 3. Pourquoi il faut sortir du “tout-GenIA”

L’engouement pour la GenIA fait oublier que tout n’a **pas besoin** d’en être.  
Et parfois, c’est même une très mauvaise idée.

### D’abord, les performances  
Les modèles génératifs ne sont pas toujours les plus efficaces.  
Sur une tâche simple, par exemple “y a-t-il un chien sur cette image ?” c'est-à-dire de la classification binaire, un modèle classique sera plus rapide, plus précis, et surtout plus stable.  
Les LLM, eux, peuvent reformuler la même idée différemment d’une exécution à l’autre, ce qui est embêtant quand on cherche de la cohérence. Voir même donner des réponses contradictoires... la GenIA n’est **ni la plus rapide ni la plus fiable** dans cette configuration.

### Ensuite, le coût  
Ces modèles sont énormes. Ils tournent sur des GPU, consomment beaucoup d’énergie, et coûtent cher.
Que ce soit en cloud ou en local, c’est la même histoire : ça chauffe, ça consomme, ça facture.  
Et pour certaines tâches simples, c’est juste… disproportionné.

### Enfin, la question éthique et environnementale  
Les données utilisées ne sont pas toujours collectées avec consentement clair. Nous n'avons aucune certitude à ce sujet mais il est propable qu'une bonne partie de ce qui existe sur internet (que ce soit publique ou non), a servi à apprendre des modèles.
De plus les modèles ne garantissent ni la vérité, ni la neutralité. On peut notamment penser aux biais d'opinions ([Santurkar et al.. 2023](https://arxiv.org/abs/2303.17548)).
Côté environnement, c’est pareil : l’entraînement d’un seul grand modèle peut émettre autant de CO₂ que plusieurs centaines de vols internationaux ([et d'autres chiffres édifiants](https://vert.eco/articles/lintelligence-artificielle-va-t-elle-donner-le-coup-de-grace-au-climat)).  
Pour donner un ordre d’idée, le calcul d’un modèle comme LLaMA 2 a consommé autant d’électricité que la ville de Paris sur plusieurs semaines (uniquement pour les GPU, sans compter le refroidissement).

Bref : des alternatives **plus sobres, plus explicables et moins coûteuses** existent. Pourquoi ne pas s’en servir ?

---

## 4. Laisser l’IA exister sans la GenIA

L’IA n’est pas un bloc unique, c’est un ensemble d’outils et de méthodes.
Les modèles génératifs, c’est un outil parmi d’autres, pas une finalité.  
Ils ont prouvé leur valeur, dans la traduction, la synthèse, la rédaction, mais ils ne doivent pas être utilisés pour tout.

Leur succès ne doit pas faire oublier la **diversité du domaine** : logique, statistiques, graphes, heuristiques, agents, apprentissage symbolique…  
Plutôt que de multiplier les couches et les milliards de paramètres, **recommençons à penser intelligemment**.  
(Et à faire sobre, parfois, ça ne fait pas de mal.)

---

## En conclusion

Après plusieurs années passées à travailler sur des modèles de traitement de la parole et de données massives, j’ai notammment appris une chose :  
il n’existe **pas une seule IA**, mais **autant d’IA que de cas d’usage**.

La vraie intelligence ne se trouve pas dans la taille des modèles, mais dans leur **pertinence**.  
Et ça, on a un peu tendance à l’oublier.

---

### Pour aller plus loin :
- [*Attention Is All You Need* — Vaswani et al., 2017](https://arxiv.org/abs/1706.03762)  
- [*The Diffusion of Generative AI* — NBER Working Paper, 2024](https://www.nber.org/papers/w34255)  
- [Cours LLM de Hugging Face (FR)](https://huggingface.co/learn/llm-course/fr/chapter1/4)  
- [*Le raisonnement symbolique*](https://www.cyberjustice.ca/2020/12/14/blogue-epistemologie-de-lia-1-lintelligence-artificielle-symbolique-quen-est-il-aujourdhui/)
- [*Explained: Generative AI’s environmental impact*](https://news.mit.edu/2025/explained-generative-ai-environmental-impact-0117)  
- [*Everyone must understand the environmental costs of AI*](https://oecd.ai/en/wonk/understand-environmental-costs)  
- [Neurosymbolic AI Workshop (NeSy’25)](https://2025.nesyconf.org/)

