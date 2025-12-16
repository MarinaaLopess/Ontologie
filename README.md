# Ontologie
Ontologie OWL développée avec Protégé
# Ontologie de la cuisine marocaine

## Présentation générale

Ce projet consiste en la conception d’une **ontologie dédiée à la cuisine marocaine**, développée dans un cadre universitaire (projet de Master). La gastronomie marocaine, riche et culturellement ancrée, constitue un domaine particulièrement pertinent pour une modélisation sémantique en raison de la diversité des plats, des ingrédients, des techniques de préparation, des traditions régionales et des contextes festifs associés.

L’objectif principal est de proposer un **modèle formel, structuré et interrogeable**, permettant de représenter et d’exploiter les connaissances culinaires marocaines à l’aide des technologies du **Web sémantique** (OWL, RDF, SPARQL).

---

## Objectifs de l’ontologie

L’ontologie vise notamment à permettre des requêtes complexes telles que :

* *Recenser les spécialités végétariennes originaires du Sud marocain*
* *Identifier les pâtisseries traditionnellement préparées lors des fêtes religieuses*
* *Localiser des plats typiques d’une région donnée*

Ce projet présente un double intérêt :

* **Technique** : application concrète des standards du Web sémantique (OWL, RDF, SPARQL)
* **Culturel** : valorisation et préservation du patrimoine gastronomique marocain grâce à une modélisation précise et contextualisée

Sur le plan pédagogique, ce travail permet de :

* maîtriser l’outil **Protégé**,
* développer des compétences en **requêtes SPARQL**,
* appliquer les principes fondamentaux du **Web sémantique**.

---

## État de l’art et réutilisation de FoodOn

Cette ontologie s’inscrit dans une logique de **complémentarité avec l’ontologie FoodOn**. Elle réutilise certains concepts génériques (ingrédients, techniques culinaires) tout en introduisant des éléments spécifiques à la culture marocaine :

* plats traditionnels et variations régionales,
* liens aux fêtes religieuses et occasions sociales,
* relations sémantiques contextualisées (origine géographique, pratiques locales).

Cette approche garantit une **interopérabilité avec FoodOn** tout en enrichissant l’écosystème existant par une modélisation culturelle fine et spécialisée.

---

## Domaine et portée

L’ontologie couvre exclusivement la **cuisine marocaine traditionnelle**, en prenant en compte :

* les plats emblématiques (tajine, couscous, pastilla, harira),
* les ingrédients distinctifs (épices, viandes, légumes, céréales),
* les méthodes de cuisson spécifiques (cuisson lente, vapeur),
* les dimensions régionales (cuisine fassie, berbère, saharienne),
* les occasions culturelles et religieuses (Ramadan, Aïd, mariages).

Elle permet :

* l’organisation sémantique de recettes,
* l’annotation intelligente de contenus culinaires,
* la recherche avancée via SPARQL,
* la recommandation contextualisée de plats.

La modélisation s’articule autour de six axes conceptuels : **plats, ingrédients, méthodes de cuisson, régions, occasions et régimes alimentaires**, tout en maintenant un équilibre entre richesse sémantique et faisabilité technique.

---

## Méthodologie de construction

La construction de l’ontologie repose sur une **approche hybride** (top-down et bottom-up) et a été réalisée avec **Protégé**.

### Étapes principales

* **Collecte des connaissances** : livres de recettes, sites spécialisés, blogs culinaires, connaissances personnelles et ontologies existantes (FoodOn)
* **Identification des concepts clés** : types de plats, ingrédients, ustensiles, méthodes de cuisson, occasions
* **Hiérarchisation des classes** : structuration arborescente (ex. Plat → PlatPrincipal, Dessert)
* **Définition des propriétés** : relations entre plats, ingrédients, régions et occasions
* **Ajout de restrictions OWL** : classes disjointes, restrictions de cardinalité
* **Documentation** : annotations `rdfs:label` et `rdfs:comment` (français / anglais)
* **Validation** : tests de cohérence à l’aide du raisonneur Pellet

---

## Modélisation ontologique

L’ontologie comprend :

* **25 classes principales**, organisées de manière thématique,
* une classe centrale *Type_de_Plat* (Desserts, Entrées, Plats_principaux),
* une spécialisation fine des ingrédients (Épices, Fruits_secs, Viandes, Légumes),
* **161 individus** représentant des plats, ingrédients et événements culturels.

Bien que les propriétés d’objet et de données soient encore en cours de formalisation, des relations clés sont prévues (ex. *utiliseIngrédient*, *estServiLors*), afin d’enrichir progressivement le modèle et de permettre des requêtes avancées.

---

## Questions de compétence et requêtes SPARQL

L’ontologie est conçue pour répondre à des questions de compétence telles que :

* identifier les plats végétariens traditionnels,
* lister les desserts marocains,
* détecter les plats utilisant un ingrédient donné,
* localiser les spécialités d’une région spécifique,
* sélectionner les plats selon leur méthode de cuisson ou une occasion particulière.

Ces requêtes démontrent la capacité de l’ontologie à croiser plusieurs dimensions (ingrédients, régions, occasions, techniques) et à restituer des connaissances culinaires riches et exploitables.

---

## Contexte académique

Projet réalisé dans le cadre d’un **Master 1**, à des fins pédagogiques et scientifiques.

## Licence

Cette ontologie est distribuée sous licence **Creative Commons Attribution 4.0 International (CC BY 4.0)**.

---

## Auteurs

* BELLAHBIB Ayoub
* BOUHAID Soukaïna  	
* CARVALHO LOPES Marina
* HACHA Mehdi 

---

## Outils utilisés

* Protégé
* OWL / RDF
* SPARQL
