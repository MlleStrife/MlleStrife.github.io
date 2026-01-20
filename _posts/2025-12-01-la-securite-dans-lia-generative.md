---
title: "La sécurité dans l'IA générative"
description: "Apporter de la sécurité dans l'usage de l'IA générative"
date: 2025-12-01
author: "MlleStrife"
tags: [cyber, genIA, utilisation consciente]
---

# La sécurité dans l'IA générative 

L’IA générative s’impose rapidement dans les entreprises à travers des outils comme ChatGPT, Gemini, Claude ou Copilot. Ces technologies transforment la manière de travailler en accélérant la création de contenu, l’analyse de données et le développement logiciel. Mais cette adoption massive s’accompagne aussi de nouveaux risques, souvent mal compris ou sous-estimés. C’est précisément pour répondre à ces enjeux qu’est née la notion de **sécurité de l’IA générative (GenAI Security)**.

La sécurité GenAI vise à protéger les organisations contre les risques liés à l’utilisation d’outils d’IA externes par les employés. Contrairement à la sécurité des modèles d’IA eux-mêmes, qui concerne l’entraînement, l’infrastructure ou les algorithmes, la sécurité GenAI se concentre sur la **phase d’utilisation**, là où les données de l’entreprise entrent réellement en contact avec des systèmes d’IA publics, le plus souvent via un navigateur web. Elle combine des contrôles techniques et des règles de gouvernance pour permettre une utilisation de l’IA à la fois productive, conforme et responsable.

---

## Pourquoi l’IA générative crée de nouveaux risques en entreprise

L’un des principaux problèmes posés par l’IA générative est la facilité avec laquelle des données sensibles peuvent être exposées. Dans un souci d’efficacité, des employés copient parfois des informations confidentielles comme des données clients, du code source, des documents financiers ou des stratégies internes directement dans des outils comme ChatGPT. Une fois ces données envoyées, l’entreprise perd en grande partie le contrôle sur leur stockage, leur conservation ou leur réutilisation potentielle. Ces données sont alors quelque part dans la nature, plus vulnérable que quand elles sont dans les mains des entreprises.

À cela s’ajoutent des enjeux de conformité réglementaire : es réglementations sur la protection des données, comme le RGPD, imposent des règles strictes sur la manière dont les informations personnelles ou sensibles peuvent être traitées. Or, la plupart des outils d’IA grand public ne sont pas conçus pour garantir, par défaut, le respect de ces exigences. Une simple requête mal formulée peut suffire à déclencher une violation réglementaire, avec à la clé des sanctions financières et une atteinte à la réputation de l’entreprise.

Un autre phénomène largement répandu est celui de l’**IA fantôme**. De nombreux collaborateurs utilisent des outils d’IA non approuvés ou des comptes personnels, souvent sans en informer les équipes informatiques. Ces usages, bien qu’animés par de bonnes intentions, échappent aux politiques de sécurité, sont absents des logs et ne sont plus controlés. Ce qui crée une absence de vision sur l'utilisation et le stockage des données sensibles, rendant impossible toute supervision réelle de l’usage de l’IA au sein de l’organisation.

Les extensions et plugins de navigateur basés sur l’IA constituent également une source de risque majeure. Pour fonctionner, ils demandent souvent des autorisations très larges, comme l’accès au contenu des pages web, au presse-papiers ou aux cookies de session. Lorsqu’ils sont développés par des tiers peu contrôlés, ces plugins peuvent être détournés pour voler des données, injecter du contenu malveillant ou détourner des sessions utilisateurs, sans être détectés par les outils de sécurité traditionnels.

---

## Une surface d’attaque en pleine expansion

L’adoption rapide de l’IA générative a modifié le périmètre de sécurité des entreprises. Là où les systèmes étaient autrefois relativement centralisés, l’IA rajoute une multitude d’outils SaaS, d’intégrations cloud et de workflows automatisés. L’IA est désormais intégrée aux suites bureautiques (Gemini ou Copilot en sont de bons exemples), aux plateformes CRM (comme Salesforce), aux outils collaboratifs et aux environnements de développement (Cursor ou Windsurf). Chaque nouvelle intégration élargit la surface d’attaque et multiplie les points de fuite potentiels.

Cette transformation est d’autant plus complexe que la majorité des interactions avec l’IA se font via le navigateur. Les outils de sécurité classiques, conçus pour les applications internes ou les réseaux d’entreprise, peinent à analyser en temps réel ce que les utilisateurs saisissent dans des interfaces web dynamiques. Ils ne voient ni les prompts envoyés aux modèles, ni le contexte dans lequel les données sont utilisées. Résultat : des informations sensibles peuvent être partagées sans qu’aucune alerte ne soit déclenchée.

---

## La gouvernance de l’IA, pilier de la sécurité GenAI

Pour être efficace, la sécurité de l’IA générative doit s’appuyer sur une gouvernance claire. Cela implique de définir des règles précises sur les outils autorisés, les types de données pouvant être utilisés et les cas d’usage acceptables. Une gouvernance bien pensée permet d’éviter l’interdiction pure et simple de l’IA, souvent contre-productive, au profit d’un cadre maîtrisé qui encourage l’innovation tout en limitant les risques.

La gouvernance joue également un rôle clé dans la visibilité et la responsabilité. En conservant une trace des interactions avec les outils d’IA et en surveillant les usages anormaux, les entreprises peuvent détecter rapidement les dérives, enquêter sur les incidents et ajuster leurs politiques au fil du temps. Dans un environnement où les outils et les usages évoluent très rapidement, cette capacité d’adaptation est essentielle.

---

## Quand la sécurité GenAI fait défaut : des conséquences bien réelles

Les incidents liés à une mauvaise gestion de l’IA générative ne sont plus théoriques. En 2023, Samsung a dû interdire l’usage de ChatGPT après que des ingénieurs ont copié du code source confidentiel dans l’outil pour corriger des bugs, exposant potentiellement des éléments critiques de propriété intellectuelle. Dans le secteur financier, des régulateurs ont ouvert des enquêtes après que des employés ont utilisé ChatGPT pour produire des analyses d’investissement et des communications clients sans contrôle, soulevant des questions de conformité et de fiabilité des informations générées. D’autres incidents ont mis en lumière le rôle des extensions de navigateur : certaines extensions ChatGPT populaires se sont révélées capables de collecter silencieusement des cookies de session et des contenus de pages web, permettant le détournement de comptes et l’exfiltration de données sans alerte des outils de sécurité classiques. Enfin, plusieurs entreprises ont découvert a posteriori une prolifération d’outils d’IA non autorisés utilisés par les équipes, chacun manipulant des données sensibles hors de tout cadre de gouvernance. Dans tous ces cas, le problème n’était pas l’IA elle-même, mais l’absence de contrôles au niveau de l’usage : aucune visibilité sur les prompts, aucune protection contre les copier-coller sensibles, et aucune gouvernance claire sur les outils autorisés.

---


## Conclusion

L’IA générative transforme durablement les modes de travail, mais elle redéfinit aussi les règles de la sécurité en entreprise. Fuites de données, non-conformité, IA fantôme et extensions non maîtrisées sont autant de défis qui nécessitent une approche nouvelle, centrée sur l’usage réel de l’IA.

---

## Pour aller plus loin

- [GenAI Security Project OWASP](https://genai.owasp.org/)
- [Samsung Bans ChatGPT Among Employees After Sensitive Code Leak](https://www.forbes.com/sites/siladityaray/2023/05/02/samsung-bans-chatgpt-and-other-chatbots-for-employees-after-sensitive-code-leak/) 
- [Considerations on Closing the Browser Security Gap, Part 3: Securing GenAI](https://www.menlosecurity.com/blog/considerations-on-closing-the-browser-security-gap-part-3-securing-genai)
- [What Is Shadow AI? How It Happens and What to Do About It](https://www.paloaltonetworks.com/cyberpedia/what-is-shadow-ai)
- [5 key considerations you need when building an AI governance framework](https://www.datagalaxy.com/en/blog/ai-governance-framework-considerations/)
- [900K Users Compromised: Chrome Extensions Steal ChatGPT and DeepSeek Conversations](https://www.ox.security/blog/malicious-chrome-extensions-steal-chatgpt-deepseek-conversations/)

---