---
layout: post
title: "Windows Logging for SOC de TryHackMe (Traduction & approfondissements)"
description: "Traduction et questions pour aller plus loin, basées sur la room 'Windows Logging for SOC' (TryHackMe)."
date: 2025-10-15
author: "MlleStrife"
logs: [Cybersécurité, SOC, Windows, Log-Analysis, TryHackMe]
---

# Windows Logging for SOC : Traduction et pistes d'approfondissement

> Cette page reprend le contenu pédagogique principal de la room *Windows Logging for SOC* ([TryHackMe](https://tryhackme.com/room/windowsloggingforsoc)) et propose des **questions supplémentaires** et exercices pour pousser la formation plus loin. Elle est destinée aux analystes SOC débutants/intermédiaires, aux analystes en réponse à incidents et aux formateurs.
Cet article montre comment on peut tirer partie d'une ressource accessible à tous.

---

## Introduction : 

Les analystes SOC passent la majorité de leur temps à trier des alertes et à chasser des menaces à partir des logs contenus dans les SIEM. Pour différencier les bons et les mauvais logs, il leur est indispensable de bien connaître les logs : à quoi ils ressemblent, comment les interpréter et à quel mauvais usage ils correspondent.
Cette room sert d'introduction à un long voyage au coeur des logs Windows, une compétence clé pour tous les analystes SOC et les professionnels DFIR.

Objectifs pédagogiques :
- Savoir localiser et interpréter les événements Windows pertinents,
- Comprendre l’intérêt de sources comme **Sysmon** et les logs PowerShell pour la détection,
- Mettre en pratique l’analyse sur des jeux de logs concrets dans d'autres rooms,
- S'entrainer à analyser les logs sur de multiples jeux de données.

Lancer la VM sur laquelle est inscrite les jeux de données. Les sections suivantes rajoutent des questions en plus de celles déjà présentes sur la room. Pour des soucis de cohérence, la suite sera en anglais.

---

### Task 2: What is Logged
- Which Event ID describes an account failing to log on?  
- How many types of logon failures are there?  
- In the **Practice-Security** log, how many occurrences of this Event ID are there?  
- How many user accounts have been tried?

---

### Task 3: Security Log: Authentification
- Is it easy to track successful logons?  
- Are all failed logons true positive alerts?  
- Which username does not exist?  
- How did the user log on as administrator? (Check the logon type)

---

### Task 4: Security Log: User Management
- What are the most likely eventID tracks in the following ? 
  - 4720 / 4738 / 4723 / 4732
  - 4726 / 4724 / 4733
  - 4722 / 4724 / 4732
- At what time was the new user account created?  
- Should this activity raise suspicion?

---

### Task 5: Sysmon: Process Monitoring
- Why should we choose Sysmon for this task?  
- What does Event ID 11 represent, and how does it differ from Event ID 15?  
- Check the provided URL on VirusTotal, what can you conclude?

---

### Task 6: Sysmon: Files and Network
- Which Event ID is relevant for tracking **file-related** events?  
- Which Event ID is relevant for tracking **network-related** events?  
- Check the domain on VirusTotal, what can you conclude?

---

### Task 7: PowerShell: Logging Commands
- PowerShell maintains a **history file**. What would be the equivalent in a Linux environment?  
- Which file has been deleted?

---

## Ma proposition de formation
A destination des équipes SOC
**Bien comprendre les logs windows (6h)**
- Rappel adminsys Windows
- Les Events ID
- Les logs de Sysmon

**Mise en application (6h)**
- Atelier : etude de cas 1
- Atelier : etude de cas 2

---

### Envie d’en savoir plus ?
Contactez-moi pour co-construire la formation qui sera la plus pertinente pour vous et/ou vos équipes.  

**Email :** [manon.macary92@gmail.com](mailto:manon.macary92@gmail.com)

---

## Pour aller plus loin

- Walkthroughs & notes publics sur la room *Windows Logging for SOC* ([ici](https://medium.com/@RosanaFS/windows-logging-for-soc-tryhackme-walkthrough-e4aa10339261), [la](https://simontaplin.net/2025/07/05/answers-for-the-tryhackme-windows-logging-for-soc-room/)) ou encore [par ici](https://medium.com/@Sle3pyHead/windows-logging-for-soc-notes-tryhackme-3faaf1e3e76f) :
- [Windows Security Log Events](https://www.ultimatewindowssecurity.com/securitylog/encyclopedia/)
