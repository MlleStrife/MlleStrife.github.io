---
title: "Utiliser Linux pour les débutants, chapitre 1 : le système de fichier"
description: "Les premiers pas dans le système de fichier pour des débutants en Linux"
date: 2025-11-15
author: "MlleStrife"
tags: [Sysadmin, linux, terminal, débutant]
---

# Utiliser Linux pour les débutants, chapitre 1 : le système de fichier

## Objectifs du cours
À la fin de ce cours, vous serez capable de : 
- Comprendre sommairement ce qu'est un système Linux,
- Utiliser efficacement des lignes de commandes pour dompter la navigation dans le système de fichier,
- Retrouver des contenus dans les fichiers,
- Connaître l'existence du man.

---

## Linux, Kézako ?

Linux est un système d’exploitation libre, basé sur le noyau Unix, largement utilisé sur les serveurs, les systèmes embarqués et le cloud notamment. Maintenant, avec l'obsolescence de certains ordinateurs personnels (merci Windows 11), on voit arriver de nouveaux utilisateurs.

Ce cours se destine principalement à ces derniers, donc je vais beaucoup utiliser Windows comme base de comparaison. Si vous êtes déjà familier avec Linux et ses distributions principales, ce post risque de vous ennuyer !

On retrouve plusieurs distributions de Linux (Debian, Ubuntu, Mint,...). Ce sont plusieurs itérations de Linux qui permettent de se focaliser sur différentes fonctionnalités. Si vous voulez une distribution grand public, je vous conseille Debian ou Ubuntu. Si vous avez une machine peu puissante, autant prendre une distribution légère comme Mint ou Bodhi. Si vous voulez absolument tout configurer pour que chaque interaction soit personnalisée, alors allez plutot sur Arch.

Ces distributions sont maintenant quasiment toute disponible avec une interface graphique (GNU), qui va vous permettre de faire à peu près tout comme sous votre Windows. Il faut juste se réhabituer à la navigation et aux différences de logiciels entre les deux systèmes d'exploitation, mais ça se fait plutot bien.

La principale différence pour un utilisateur c'est d'utiliser son ordinateur sans interface graphique. Car oui, il existe des interfaces graphiques, mais la richesse et la puissance de Linux vient de son interface en ligne de commande. Vous savez ces représentations que l'on voit dans les films de hackers devant un écran noir plein de mot ? Et bien on est en plein dedans. Maintenant cette introduction a trop durée, il est temps de parler de l'administration Linux et donc de ligne de commande.

## Le terminal, la maison de toutes les commandes

Pour utiliser les lignes de commandes, il faut pouvoir les écrire quelque part. C'est pour cela que l'on utilise un terminal. C'est comme une page blanche sur un éditeur de texte, sauf que lorsqu'on revient à la ligne, le terminal nous répond puis nous rend la main. Pour faire les exercices pratiques, nous allons utiliser [ce site](https://www.terminaltemple.com/) .
Illustrons ce que nous venons de dire en tapant ` echo Bonjour !` puis en appuyant sur entrée. Le terminal vous répond `Bonjour !` . Oui vous venez de faire votre première ligne de commande : `echo` est une commande qui affiche une ligne de texte.

## Naviguer dans le système de fichier

Sous Windows (ou en utilisant une interface graphique) pour aller voir ce qu'il y a dans un dossier (que l'on nomme répertoire ici), il suffit de le trouver et de cliquer dessus. En interface de commande on va avoir plusieurs commandes permettant de se déplacer, de créer, de supprimer, de lire et d'écrire des fichiers:

| Commande 	| Description                                                      	| Exemple                          	|
|----------	|------------------------------------------------------------------	|----------------------------------	|
| ls       	| permet de lister les fichiers dans le répertoire courant         	| ls                               	|
| cd       	| permet de changer de répertoire                                  	| cd FOLDER                        	|
| cat      	| permet de lire un fichier texte dans le répertoire courant       	| cat FICHIER                      	|
| touch    	| permet de créer un fichier                                       	| touch README.txt                 	|
| rm       	| permet de supprimer un fichier                                   	| rm README.txt                    	|
| cp       	| copier un fichier/répertoire                                     	| cp ancien.txt nouveau.txt        	|
| mv       	| déplacer un fichier/répertoire. Peut être utilisé pour renommer. 	| mv ancien.txt FOLDER/nouveau.txt 	|


Toujours en utilisant le [terminal](https://www.terminaltemple.com/) , répondez aux questions :
- Comment y a t il de répertoire courant ?
- Aller dans le répertoire Documents. Que contient ce dossier ?
- Un fichier devrait retenir votre attention. Lisez-le. Quel animal est utilisé dans le plan ?
- Créer un fichier `le-plan-version-fr.txt`, dupliquer-le, puis supprimer le fichier anglais.rm !

## L'arborescence, la racine et le mouvement

Super, vous avez utilisé avec succès vos premières commandes. Maintenant revenons voir ce qu'il y a dans le dossier Music. Mince, il faut apprendre à revenir dans le répertoire précédent. Pour cela il faut savoir une chose. Si vous faites un `ls -a` (oui parce qu'on peut donner des options aux commandes, ici -a veut dire all, donc de tout afficher), vous allez voir qu'il y a deux trucs bizarres : un point `.` et deux points `..` . Le système de fichier est en arborescence, c'est à dire qu'il suit une logique d'arbre : on part de la racine (`/` on verra ça plus tard), et on descend dans les branches (les répertoires), pour aller voir les feuilles (les fichiers). Le répertoire courant est représenté par le `.` ! Donc `ls` et `ls .` donne les mêmes résultats. Pour redescendre dans l'arbre, on utilise le `..` qui représente le répertoire parent (la branche). On peut remonter jusqu'à la racine comme ça, avec le `cd ..`.

Toujours en utilisant le [terminal](https://www.terminaltemple.com/) , répondez aux questions :
- Retourner dans le répertoire initial et aller voir ce qu'il y a dans Music.
- Remonter jusqu'à la racine (`/`), comment y-a-t-il de répertoires ?

## Mais où j'ai mis mon plan de conquête du monde ?

Super, on s'est bien déplacé dans le système de fichier. Mais il était où déjà notre plan français ? Plutot que de chercher un à un les répertoires de notre système, nous pouvons utiliser une super commande du nom de `find`. Cette dernière permet de trouver un fichier ou un répertoire dans l'arborescence, sans en connaître le chemin direct. Il va falloir il dire ce qu'on veut chercher... On va donc reparler des options ! On peut tout trouver avec find en utilisant `-name` :
`find . -name [nom_fichier]` On cherche dans le répertoire courant `.` (ou ailleurs), tout ce qui a pour nom `nom_fichier`. 

Zut mais le fichier que je veux voir est trop long, je voulais le nom de mon animal de compagnie uniquement moi. Par contre je sais que j'avais écrit le mot HAMSTER devant son nom dans mon fichier. Pas de panique ! Nous pouvons utiliser la commande `grep` qui va nous permettre de retrouver ce qu'il y a dans un fichier :
`grep "HAMSTER" [nom_fichier]` On cherche dans `nom_fichier`, la ligne avec le mot `"HAMSTER"`. Comme tout ceci est un peu plus compliqué, je vous propose de continuer ensemble cette formation si elle vous plaît dans un autre module !

## Le man : le manuel 

Il existe une multitude de commande avec une quantité énorme d'option. Mais pour les découvrir et savoir les utiliser, nous avons le man. Il s'agit du man de chaque commande avec la description de la commande, comment on l'utilise, quelles sont les options, des exemples d'utilisation et des commandes approchantes. Il est disponible en ligne de commande `man [commande]` directement dans le terminal ou sur internet (par exemple en [français](https://www.man-linux-magique.net/))

---

## Ma proposition de formation (32h) : 
A destination des débutants Linux

**Partie 1 : Fondamentaux de Linux**

- Présentation de Linux et de l’open source
- Distributions Linux et cas d’usage
- Installation et prise en main du système
- Découverte du terminal et du shell
- Commandes essentielles
- Arborescence et gestion des fichiers
- Éditeurs de texte sous Linux

**Partie 2 : Administration de base**

- Gestion des utilisateurs et des groupes
- Permissions et droits d’accès
- Gestion des processus et des services
- Installation et mise à jour des logiciels

**Partie 3 : Réseau et sécurité de base**

- Configuration réseau simple
- Pare-feu et notions de sécurité
- Bonnes pratiques d’administration

**Partie 4 : Automatisation et maintenance**

- Planification des tâches
- Introduction au scripting shell
- Sauvegarde et surveillance basique du système

---

### Envie d’en savoir plus ?
Contactez-moi pour co-construire la formation qui sera la plus pertinente pour vous et/ou vos équipes.  

**Email :** [manon.pinel92@gmail.com](mailto:manon.pinel92@gmail.com)

---