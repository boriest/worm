# Sommaire
## Introduction
* [Présentation de l'entreprise](intro/presentation.md)
  * [Imakumo](intro/presentation.md#Imakumo)
  * [ServiceNow](intro/presentation.md#ServiceNow)
  * [Missions](intro/presentation.md#Missions)
* [Contexte du projet](intro/context.md)
  * [Eve](intro/context.md#eve)
  * [Gestion de planning](intro/context.md#planning)
* [Sujet du mémoire](subject/subject.md)

## Programmation fonctionnelle
* [Introduction]()
  * [Concepts]()
  * [Pourquoi la programmation fonctionnelle]()
  * [Langages]()
* [Théorie]()
  * [...]()
* [État de l'art en JavaScript]()
  * [...différentes librairies...]()

## Un cas concret: une application de gestion de planning
* [Pourquoi utiliser la programmation fonctionnelle]()
  * est-ce un bon choix ici ? (niveaux hétérogènes de dev, temps de formation)
* [Analyse de la mise en oeuvre]()
  * formation des consultants, maintenabilité
  * quand choisir la programmation fonctionnelle

## Bibliographie
* [Ouvrages](biblio/ouvrages.md)
* [Sites internet](biblio/web.md)

# Introduction
## Présentation de l'entreprise
### Imakumo
Société de service informatique. Créée 2010.
Rapid growth.

### ServiceNow
"ERP" pour l'it
automatisation des processus informatiques (ITIL)

### Missions
Consultant.
Intégration, support, conseil, etc

## Contexte du projet
La mission intervient dans le cadre d'un projet interne, dont le but est à terme de développer un ERP dans ServiceNow.

### Eve
EVE est le nom de l'outil développé en interne, dans une instance ServiceNow.
Son but est de reprendre les fonctionalités d'un ERP classique, pour une utilisation interne.
Il vise à :
* **réduire les coûts** en décommissionnant des outils tiers (e.g. Spot)
* **automatiser** un certain nombre de traitements (e.g. notes de frais, facturation)
* **centraliser** les processus (e.g. facturation, timesheets)

### Gestion de planning
Le module sur lequel est basé ma mission est celui de la gestion des projets, à la fois internes et externes.
Il est utilisé en interne par les managers afin de positionner des consultants sur des missions, et par les consultants pour consulter leurs plannings.
La partie dont je suis en charge consiste à développer deux vues :
* une vue manager, depuis laquelle ils auront une vue d'ensemble sur les plannings des projets et des consultants
* une vue consultant, depuis laquelle ils auront les informations sur les missions plannifiées par jour
  * cette vue doit permettre de valider ou non une mission effectuée, qui alimentera une timesheet

Ce module est actuellement disponible sur un autre outil interne, qui est implémenté dans une instance ServiceNow.
Cependant, la technologie utilisée est vieillissante, et peu pratique (vues statiques, long temps de chargement, etc).
