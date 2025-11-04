---
layout: post
title: "La fatigue des SOC : pourquoi elle arrive, pourquoi c’est dangereux, et comment la réduire"
description: "Un tour d’horizon humain et technique sur la fatigue des analystes SOC, les causes, et les moyens concrets de la limiter."
date: 2025-09-15
tags: [cyber, soc, formation]
author: "MlleStrife"
---

# La fatigue des SOC : pourquoi elle arrive, pourquoi c’est dangereux, et comment la réduire

Si tu bosses en SOC, tu connais la rengaine : des milliers d’alertes par jour, des tickets qui s'empilent, des playbooks pas à jour, et ce sentiment latent que tu cours après quelque chose que tu n’attraperas jamais.
Ce n’est pas juste “la vie en sécurité” : c’est **de la fatigue, et parfois du burnout**. En plus d'être critique pour les individus, ça mine également l’efficacité de la défense.

---

## L’état des lieux (spoiler : c’est du sérieux)

Les chiffres parlent d’eux-mêmes.  
De nombreuses études soulignent que les SOC se sentent débordés. [Ici](https://www.helpnetsecurity.com/2023/07/20/soc-analysts-tools-effectiveness/) on rapporte que **plus de 65 % des alertes sont ignorées chaque jour**. Les analystes SOC déclarent ne pas parvenir à suivre le volume d’alertes quotidien.  
Et près de 70 % [citent](https://newsroom.trendmicro.com/2021-05-25-70-Of-SOC-Teams-Emotionally-Overwhelmed-By-Security-Alert-Volume) le **trop gros volume d'alertes**, le **manque d’automatisation** et la **prolifération des outils** comme sources majeures de stress.

L’étude académique [*Alert Fatigue in Security Operations Centres: Research Challenges and Opportunitues* [Tariq and al..]](https://dl.acm.org/doi/full/10.1145/3723158) va plus loin : elle montre que l’exposition répétée à des alertes non pertinentes **désensibilise les analystes** et **augmente le risque de manquer une véritable menace**.

Même constat du côté des éditeurs de systèmes cyber (Palo Alto, Cybereason, Swimlane,...) : la fatigue des SOC issue des alertes (qu'on appelera alert fatigue pour plus de simplicité) engendre une **perte de réactivité**, un **taux élevé d’erreurs**, et une **hausse du MTTR** (temps moyen de remédiation). C'est donc une grosse problématique, qui existe depuis des années et qui n'est toujours pas réglée.

---

## Pourquoi ça arrive (encore)?

On peut résumer les causes en quatre grandes familles :

1. **Volume & bruit (noise)** : trop d’alertes, trop de faux positifs. Les règles non ajustées des SIEM ou EDR génèrent du bruit inutile.  
2. **Manque de contexte** : une alerte sans enrichissement (qui, quoi, quand, où, comment ) oblige à des recherches manuelles chronophages.
3. **Pléthores d'outils** : plusieurs outils, plusieurs consoles et pas (ou peu) d’intégration, de corrélation entre eux. Résultat : on perd beaucoup de temps à naviger et à retrouver les bonnes informations et on se fatigue, on se démotive.  
4. **Sous-effectif et/ou process fragiles** : quand on combine des équipes épuisées, des horaires décalés, un turnover élevé et des playbooks obsolètes, on se retrouve avec le cocktail parfait pour la saturation.

---

## Pourquoi c’est dangereux

On peut assez facilement se rendre compte de la dangerosité d'une équipe SOC qui n'arrive plus à suivre. On va passer à coté des vraies alertes, ce qui pose un problème opérationnel très important. Et si on va sur le terrain des alertes critiques ignorées, on parle alors d'incident non contenu, ce qui a un impact financier mais également qui risque de ternir la réputation de l'entreprise.
Lorsque la personne atteint la zone critique du burnout, on perd des personnes qui sont formées, qui ont l'habitude de travailler avec nos outils et les types d'alertes critiques de l'entreprise. Le turnover coûte cher et fait perdre un temps précieux.

---

##  Réduire la fatigue : principes simples plein de bon sens

1. **Réduire le bruit avant d’automatiser**
   Un SIEM mal tuné sur des logs inutiles est un SIEM qui ne va pas assez aidé les équipes. Un modèle d’automatisation amplifie les erreurs si les règles d’origine sont mauvaises.

2. **Donner du contexte à chaque alerte**  
   Pour éviter aux équipes de faire un fastidieux travail de recherche et enrichir manuellement les alertes, on peut mettre en place un enrichissement automatique. Remplir les fameux qui quoi ou quand.

3. **Prioriser intelligemment**
   Classer les alertes par impact business et vraisemblance, pas juste par timestamp. Ça peut sembler bizarement de le spécifier, mais ce n'est pas toujours le cas.

4. **Se référer à un framework type Mitre Att&ck**  
   Pouvoir situer l'alerte dans les cases TTPs (Tactics, Techniques and Procedures) du Mitre Att&ck par exemple permet de cibler ce qu'on recherche et quelles sont les probables prochaines étapes. On va donc réduire le champ de recherche et qui dit moins de recherche à faire dit moins de fatigue cognitive.

5. **Automatiser ce qui est fatigeant (pas ce qui intéressant)**  
   Triage, enrichissement, quarantaines basiques sans intervention humaine par suite de règles pré-établies ou modèles appris ? Bien sur. Décision stratégique sans la supervision humaine ? Jamais.  

6. **Prendre soin des analystes**  
   Formation continue, mentoring, plages sans interruptions, rotations sur les horaires de nuit. 
   Gartner et d'autres acteurs parlent désormais de [**human-centered SOCs**](https://www.cyberdefensemagazine.com/gartners-calling-for-a-human-centric-approach-to-cybersecurity-heres-how-to-implement-it/). Les analystes sont en première ligne face aux alertes, il faut leur permettre de pouvoir continuer de travailler dans les meilleurs conditions possibles.

Cette liste n'est pas triée par ordre d'importance ou de priorité évidemment, ce sont des principes tout aussi important les uns que les autres.
   
---

## Dans les faits : passer à l’action

### Les objectifs court termes (1 à 4 semaines)
- Audit des règles SIEM les plus bruyantes. Selon les moyens techniques et financiers, les 20, 50, 100 plus fréquentes peuvent être analysées pour être que ces alertes, si elles ne sont pas critiques, puissent être traitées automatiquement.
- Audit du niveau technique des analystes et mise en place de formations appropriées pour fluidifier leur travail et donc réduire leur fatigue.
- Ajout d’un enrichissement automatique minimal : propriétaire + contexte IP + réputation. Plus on a de question *qui quoi quand où* de répondus automatiquement, plus on enlève du travail fatiguant aux analystes.
- Favoriser la communication et l'entraide au sein de l'équipe. On se fatigue moins à plusieurs, on peut vite se sentir débordé seul.

### Les objectifs à moyen terme (2 à 12 mois)
- Implémenter une approche *detection engineering* comme le MITRE ATT&CK.  
- Automatiser les tâches de triage via des règles qui sont comprises par l'équipe SOC.  
- Créer un parcours de formation continue pour les analystes, car les menaces évoluent en permanences.
- Monitorer l'état de l'équipe en se basant sur des KPI chiffrés (nombre d'alertes journalières, nombre de faux positifs, suivi du MTTR, nombre d'alertes enrichies automatiquement,enquête régulière du niveau de fatigue et/ou de satisfaction de l'équipe SOC,...)

---

## Ma proposition de formation : 
A destination des managers SOC

**Comprendre le problème (6h)**  
- Les chiffres de la fatigue SOC  
- Audit de quelques alertes 
- Atelier 1 : catégoriser les sources de bruit

**Agir concrètement (6h)**  
- Détection engineering : démonstration MITRE  
- Atelier 2 : SOAR automatiser un triage basique  
- Atelier 3 : construire un plan d’action 90 jours

A destination des équipes SOC
**Comprendre le problème (8h)**  
- Les chiffres de la fatigue SOC  
- Exemple : des alertes inutiles et le temps de résolution
- Atelier 1 : Priorisation des alertes, enrichissement manuel

**Agir concrètement (6h)**  
- Détection engineering : démonstration MITRE
- Atelier 2 : utilisation et construction de règles d'automatisation pour enrichissement
- Atelier 3 : Refaire un atelier 1 avec l'utilisation des règles définies en atelier 2

---

### Envie d’en savoir plus ?
Contactez-moi pour co-construire la formation qui sera la plus pertinente pour vous et/ou vos équipes.  

**Email :** [manon.macary92@gmail.com](mailto:manon.macary92@gmail.com)

---

## Pour aller plus loin

- [SANS SOC Survey 2024](https://www.sans.org/white-papers/soc-survey-2024/)  
- [SANS SOC Survey 2025](https://www.sans.org/white-papers/sans-2025-soc-survey)
- [*Alert Fatigue in Security Operations Centres: Research Challenges and Opportunitues* [Tariq and al..]](https://dl.acm.org/doi/full/10.1145/3723158)
- [*MITRE - 11 Strategies of a World-Class Cybersecurity Operations Center*](https://www.mitre.org/sites/default/files/2022-04/11-strategies-of-a-world-class-cybersecurity-operations-center.pdf)  
- [*Warning Signs of Security Analyst Burnout & Ways to Reduce it.* (Swimlane Blog)](https://swimlane.com/blog/analyst-burnout-signs/)  
- [*Gartner’s Calling for a Human-Centric Approach to Cybersecurity – Here’s How to Implement It* (Gartner)](https://www.cyberdefensemagazine.com/gartners-calling-for-a-human-centric-approach-to-cybersecurity-heres-how-to-implement-it/)  
- [*What is Security Alert Fatigue* (Palo Alto)](https://www.paloaltonetworks.com/cyberpedia/how-to-reduce-security-alert-fatigue.)

