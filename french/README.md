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

## Data Catalog Features
A data catalog is a listing of available data, with each catalog entry corresponding to one or more data resources. It usually includes high-level information for each dataset, such as Title, Description, Release Date, Category(-ies), and Keyword(s).

### Customers
* must be able to search for datasets by one or more terms contained in dataset metadata
* must be able to browse or explore data by category
* must be able to download the catalog in a machine-readable format compatible with the [common core metadata schema](https://project-open-data.cio.gov/v1.1/metadata-resources/) from a well-known address (typically /data.json)
* must be able to view a summary page for each dataset which details data resources, metadata, and other relevant documentation
* may be able to search for datasets by terms contained in the data

### Publishers
* must be able to add, edit, or remove catalog entries
* may be able to mark catalog entries as private so they are not visible to the public

### Administrators
* must be able to create, edit, and retire metadata categories
* must be able to configure default sorting for data catalog
* must be able to configure global settings for data catalog, including color theme, branding/logo, titling.
* may be able to configure additional global settings for data catalog, including custom Cascading Style Sheets (CSS), homepage display elements and layout, displayed catalog elements, and more.

## Data Storage & Management Features

### Customers
* must be able to download stored data in bulk
* may be able to access stored data through a REST API

### Publishers
* must be able to create new data resources
* must be able to replace or update existing data resources

### Administrators
* must be able to manage permissions for other administrators and publishers

## Data Presentation Features

### Customers
* must be able to preview data resources using an through their internet browser (for example, through a rows-and-columns grid or a map)
* may be able to visualize data resources in a graphical way, including maps, graphs, charts, etc.
* may be able to save visualizations with configuration settings for future viewing

### Publishers
* may be able to create data visualizations and make them accessible through the data catalog or data resource page(s)

### Administrators
* may be able to control whether customer-created data presentations are visible to other customers

## Community Features

### Customers
* must be able to provide comments and feedback on individual data resources
* may be able to nominate data resources for public release
* may be able to provide comments and feedback on the data catalog

### Publishers
* must be able to view customer-nominated data resources
* may be able to update the status of customer-nominated data resources
* may be able to respond to customer-nominated data resources
* may be able to view and respond to customer comments and feedback
* may be able to review and approve visibility of customer comments and feedback

### Administrators
* must track and analyze customer feedback

## Accounts and Profiles

### Customers
* may be able to register for an account with an email address
* may be able to create, edit, or remove profile information which may be accessible to other customers

### Publishers
* may be able to grant specific, registered customers permission to access specific data resources that are owned by that publisher

### Administrators
* must be able to manage permissions for other administrators and publishers
* must be able to disable customer accounts (if customer accounts are a feature of the portal)

## Non-Role Requirements
The following requirements are general technical requirements which either don’t require a specific role or apply to all roles.

* Data resources must be available for download in the format in which they were originally published on the portal
* API calls which are invalid or fail must return the appropriate HTTP response status code (404, 500, etc) and status message
* The portal must be accessible through a city-provided internet domain name (e.g. `data.somecity.gov`)
* Transport Layer Security (TLS) must be used for account registration, logging in, and all actions performed by publishers and administrators
* Web pages must be accessible on large-screen devices (desktop computers, laptops, etc.)
* Web pages may be accessible on small-screen devices (mobile/smart phones, tablets, etc.)
