# Collection Postman de requête Apidae

Cette collection Postman permet de se familiariser avec les différents types d'API que propose Apidae au travers d'exemples variés.

### La liste des exemples disponibles

- **APIs de consultation**
  * Recherche d'un objet touristique
  * Recherche d'objets touristiques
  * Agenda
  * Consultation du référentiel
  * Consultation des membres
  * Consultation des utilisateurs
  * Multi-horaires

- **Single Sign On (SSO)
- **APIs d'écriture
  * Création
  * Modification
  * Suppression

- **APIs de métadonnées
- **Appel de notifications

##### <span style="color:red"> ATTENTION BUG : </span>

La suppression de descriptifs n'est pas encore fonctionnelle. 

### Liste des paramètres

Avant toute utilisation de la collection, il est important de renseigner les variables de collection pour le bon fonctionnement des requêtes. 

1. Survolez votre collection avec le pointeur, puis cliquez sur les 3 points et enfin sélectionnez `edit` dans le menu déroulant

<img src="variable_1.PNG" style="zoom: 33%;" />

2. Rendez vous dans l'onglet `Variables` (1) puis dans un second temps vous n'aurez plus qu'à remplacer les `XXX` par vos valeurs (2)

   <img src="variables_2.png" style="zoom: 33%;" />

**apiKey**: La clé d'API

**projetId**: L'identifiant du projet

**selectionIds**: Les identifiants des sélections d’objets à récupérer (les identifiants doivent être séparés par des virgules : XXX,YYY)

**client_id**: L'identifiant du client utilisé pour un projet de type `SSO`

**secret**: Le secret associé au client précédemment renseigné

**access_token**: Le token utilisé pour configurer l'`Authorization`(voir documentation sur la configuration des tokens)

**client_id_ecriture**: L'identifiant du client utilisé pour un projet de type `API d'écriture`

**secret_ecriture**: Le secret associé au client précédemment renseigné

**access_token_ecriture**: Le token utilisé pour configurer l'`Authorization`(voir documentation sur la configuration des tokens)

**client_id_meta**: L'identifiant du client utilisé pour un projet de type `API de métadonnées`

**secret_meta**: Le secret associé au client précédemment renseigné

**access_token_meta**: Le token utilisé pour configurer l'`Authorization`(voir documentation sur la configuration des tokens)



##### <span style="color:red">ATTENTION : </span>

Il existe deux environnements : la **Production** et la **Pré-production**. Pour les APIs de consultation ainsi que le SSO vous pouvez utiliser l'environnement de `Production` mais pour les autres type de requête il faut utiliser celui de `Pré-Production`.

Enfin il peut y avoir des problèmes avec les identifiants des objets déjà présents car vos projets ne les possèdent pas forcément en cas de problème il vous suffit de remplacer cet id par un des votre.

**Toutes les requêtes sont documentées sur leur utilité ou encore comment les construire avec des paramètres remplaçables en cas de d'incompréhension ou si vous cherchez des informations complémentaires vous pouvez vous rendre sur le site d'aide aux développeurs de la plateforme : http://dev.apidae-tourisme.com/fr/documentation-technique/v2

