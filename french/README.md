# Les Exigences d’un portail Open Data

### Introduction
Ce document contient une liste des fonctionnalités requises pour aider les gouvernements à évaluer, élaborer (ou de se procurer), déployer et lancer un site web Open Data (portail).

### Terms
Les termes suivants sont utilisés pour indiquer l'importance.

* **Doit **  désigne une exigence qui est essentiel à la mise en œuvre et la réussite du portail Open Data. Si cette exigence n’est pas remplie, elle entravera de manière significative l'utilisation et la gestion du site.
* **Peut** désigne une exigence qui est facultative, mais fortement souhaitable pour le succès.

### Les rôles
Les rôles suivants sont utilisés dans ce document pour identifier à qui chaque exigence est pertinente. Ils ne sont pas destinés à refléter un système d'autorisation, ce qui pourrait être mis en œuvre par une solution technologique.

* Un **client** est toute personne qui visite le portail pour chercher et accéder aux données du portail Open Data.
* Un **éditeur** est un employé du gouvernement qui est responsable de la publication de données ou de la mise à jour du contenu du portail.
* Un **administrateur** est un employé du gouvernement qui gère les options techniques et la configuration du portail, tels que les thèmes visuels, les exigences de métadonnées, etc.

Généralement, un éditeur peut faire tout ce qu'un client peut faire, et un administrateur peut faire tout ce qu'un éditeur peut faire dans le portail.

## Caractéristiques du catalogue de données
Un catalogue de données est une liste des données disponibles, chaque entrée du catalogue correspondant à une ou plusieurs ressources de données. Il inclut des informations de haut niveau pour chaque ensemble de données, telles que le titre, description, date de sortie, Catégorie (s) et Mot-clé (s).

### Clients
* Doit être capable de rechercher les données par un ou plusieurs termes contenus dans les métadonnées de la liste des données.
* Doit être capable de naviguer ou explorer les données par catégorie.
* Doit être capable de télécharger le catalogue dans un format lisible par une machine compatible avec le « schéma commun de métadonnées de base » à partir d'une adresse bien connue (/data.json comme exemple).
* Doit être capable d'afficher une page de résumé pour chaque liste de données qui détaille les ressources de données, les métadonnées et les autres documents pertinents.
* Peut être capable de rechercher des listes de données par des termes contenus dans les données.

### Publishers
* Doit être capable d'ajouter, modifier ou supprimer des entrées de catalogue
* Peut être capable de marquer les entrées de catalogue que privé, afin qu'ils ne sont pas visibles pour le public.

### Administrateurs
* Doit être capable de créer, éditer, et de retirer des catégories de métadonnées
* Doit être capable de configurer le tri par défaut pour le catalogue de données
* Doit être capable de configurer les paramètres globaux pour le catalogue de données, y compris thème de la couleur, l'image de marque / logo, titrage.
* Peut être capable de configurer les paramètres globaux supplémentaires pour le catalogue de données, y compris les feuilles de style (CSS), les éléments d'affichage de la page d'accueil et la mise en page, affichage des éléments de catalogue, et plus encore.

## Caractéristiques de stockage et gestion des données

### Clients
* Doit être capable de télécharger des données stockées en vrac.
* Peut être capable d'accéder aux données stockées via une API REST.

### Éditeurs
* Doit être capable de créer des nouvelles ressources de données.
* Doit être capable de remplacer ou de mettre à jour les ressources de données existantes.

### Administrateurs
* Doit être capable de gérer les autorisations pour d'autres administrateurs et éditeurs.

## Caractéristiques de présentation des données

### Clients
* Doit être capable de pré visualiser les ressources de données en utilisant un biais de leur navigateur Internet (par exemple, à travers une grille lignes-et-colonnes ou d'une carte).
* Peut être capable de visualiser les ressources de données de manière graphique, y compris des cartes, des graphiques, des tableaux, etc.
* Peut être capable de sauver des visualisations avec des paramètres de configuration pour un visionnement ultérieur.

### Éditeurs
* Peut être capable de créer des visualisations de données et les rendre accessibles à travers la page du catalogue de données ou une ressource de données.

### Administrateurs
* Peut être capable de contrôler si les présentations de données créées par le client sont visibles à d'autres clients.

## Caractéristiques de la Communauté

### Clients
* Doit être capable de fournir des commentaires sur les ressources de données individuels.
* Peut être capable de nommer les ressources de données pour la diffusion publique.
* Peut être capable de fournir des commentaires sur le catalogue de données.

### Éditeurs
* Doit être capable d'afficher les ressources de données désignées par le client.
* Peut être capable de mettre à jour l'état des ressources de données désignées par le client.
* Peut être capable de répondre à des ressources de données désignées par le client.
* Peut être capable de visualiser et de répondre aux commentaires des clients.
* Peut être capable d'examiner et d'approuver la visibilité des commentaires des clients.

### Administrateurs
* Doit être capable de suivre et d’analyser les commentaires des clients.

## Comptes et Profils

### Clients
* Peut être capable de créer un compte avec une adresse e-mail.
* Peut être capable de créer, modifier ou supprimer des informations de profil qui peut être accessible à d'autres clients.

### Éditeurs
* Peut être capable d’assurer un accès spécifique pour les clients enregistrés à des ressources des données spécifiques qui sont détenues par cet éditeur.

### Administrateurs
* Doit être capable de gérer les autorisations pour d'autres administrateurs et éditeurs.
* Doit être capable de désactiver les comptes des clients (si les comptes des clients sont une caractéristique du portail).

## Autre exigences
Les exigences suivantes sont des exigences techniques générales qui ne sont pas nécessaire pour un rôle spécifique.

* Ressources de données doivent être disponibles pour le téléchargement dans le format dans lequel ils ont été publiés sur le portail.
* Les appels d'API qui sont invalides doivent retourner le code de réponse HTTP appropriée d'état (404, 500, etc.) et un message d'état.
* Le portail doit être accessible via un nom de domaine Internet de la ville prévue (par exemple data.somecity.gov).
* Transport Layer Security (TLS) doit être utilisé pour l'enregistrement des comptes, connexion aux comptes, et toutes les actions effectuées par les éditeurs et les administrateurs.
* Les pages Web doivent être accessibles sur les appareils à grand écran (ordinateurs de bureau, ordinateurs portables, etc.).
* Les pages Web peuvent être accessibles sur les appareils à petit écran (téléphones mobiles intelligents /, comprimés, etc.).
