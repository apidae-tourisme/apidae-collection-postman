# Collection Postman de requêtes Apidae

Cette collection [Postman](https://www.postman.com/) permet de se familiariser avec les différents types d'API que propose [Apidae](https://www.apidae-tourisme.com/) au travers d'exemples variés. Il existe également deux environnements : la **Production** et **Cooking** qui est un environnement de test. 
Pour les APIs de consultation ainsi que le SSO vous pouvez utiliser l'environnement de `Apidae-Production` mais pour les autres type de requête il faut utiliser celui de `Apidae-Cooking-...`.

### La liste des exemples disponibles

- **APIs de consultation** - [documentation](http://dev.apidae-tourisme.com/fr/documentation-technique/v2/api-de-diffusion)
  * Projets numériques
    * Lecture des sélections d'un projet
    * Lecture d'un objet touristique
    * Recherche d'objets touristiques
    * Agenda
    * Consultation du référentiel
    * Consultation des collaborateurs
    * Consultation des membres
    * Consultation des utilisateurs
  * Service de consentement
    * Récupération des ensembles d'offres
    * Recherche - list-identifiants
    * Recherche - list-objets-touristiques
    * Récupération d'un objet touristiques - get-by-id
    * Récupération d'un objet touristique enrichi - enrich
    * Agenda Simple - list-identifiants
    * Agenda Simple - list-objets-touristiques
    * Agenda Détaillé - list-identifiants
    * Agenda Détaillé - list-objets-touristiques
    * Recherche - list-objets-touristiques - Query
  * Multi-horaire
  * Apidae Photo
  * Appel enrichi
* Multi-horaires
  
- **Single Sign On (SSO)** - [documentation](http://dev.apidae-tourisme.com/fr/documentation-technique/v2/oauth/single-sign-on)
- **APIs d'écriture** - [documentation](http://dev.apidae-tourisme.com/fr/documentation-technique/v2/api-decriture)
  * Création
  * Modification
  * Suppression
  * Autorisation de Modification
- **APIs de métadonnées** - [documentation](http://dev.apidae-tourisme.com/fr/documentation-technique/v2/metadonnees)
- **Appel de notification** - [documentation](http://dev.apidae-tourisme.com/fr/documentation-technique/v2/exports/notificationi-traitement-confirmation)



### Liste des paramètres

Avant toute utilisation de la collection, il est important de renseigner les variables de collection pour le bon fonctionnement des requêtes. 

1. Survolez votre collection avec le pointeur, puis cliquez sur les 3 points et enfin sélectionnez `edit` dans le menu déroulant

<img src="screenshot/variable_1.PNG" style="zoom: 33%;" />

2. Rendez vous dans l'onglet `Variables` (1) puis dans un second temps vous n'aurez plus qu'à remplacer les `XXX` par vos valeurs (2)

   <img src="screenshot/variables_2.png" style="zoom: 33%;" />

**projetId** : L'identifiant du projet numérique Apidae

**selectionIds** : Les identifiants des sélections d’objets, propre aux projets numériques Apidae, à récupérer (les identifiants doivent être séparés par des virgules : XXX,YYY)

**projectId** : L'identifiant du projet, propre au service de consentement.

**searchId** : Identifiant d'un ensemble d'offres (propre au service de consentement)

**apiKey** : La clé d'API

**client_id** : L'identifiant du client utilisé pour un projet de type `SSO`

**secret** : Le secret associé au client précédemment renseigné

**access_token** : Le token utilisé pour configurer l'`Authorization` ([voir documentation sur la configuration des tokens](./Documentation_Token_Postman.md))

**client_id_ecriture **: L'identifiant du client utilisé pour un projet de type `API d'écriture`

**secret_ecriture** : Le secret associé au client précédemment renseigné

**access_token_ecriture **: Le token utilisé pour configurer l'`Authorization` ([voir documentation sur la configuration des tokens](./Documentation_Token_Postman.md))

**client_id_meta** : L'identifiant du client utilisé pour un projet de type `API de métadonnées`

**secret_meta **: Le secret associé au client précédemment renseigné

**access_token_meta** : Le token utilisé pour configurer l'`Authorization` ([voir documentation sur la configuration des tokens](./Documentation_Token_Postman.md))



##### <span style="color:red">ATTENTION : </span>

Il peut y avoir des problèmes avec les identifiants des objets déjà présents car vos projets ne les possèdent pas forcément, en cas de problème il vous suffit de remplacer cet id par un des votre.

**Toutes les requêtes sont documentées sur leur utilité et leur construction avec des paramètres remplaçables. En cas de d'incompréhension ou si vous cherchez des informations complémentaires n'hésitez pas à consulter le [site d'aide aux développeurs](http://dev.apidae-tourisme.com/fr/documentation-technique/v2).**

