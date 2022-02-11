# mary_gregoire_B_2022_docker
 
[![Branche principale](https://github.com/Greg-Orius/mary_gregoire_B_2022_docker)]

Ce projet scolaire a pour but de faire tourner une application Web se basant sur React à l'aide de NodeJS et MongoDB dans de multiples containers Docker.

---

## Sommaire

1. [Pré-requis]
2. [Utilisation]
   * [Déployer le stack]
   * [Suppression]
   * [Tester l'application]
3. [Configuration Docker]
   * [Frontend]
   * [Backend]
   * [docker-compose.yml]
4. [Diagramme d'architecture]


## Pré-requis

* [Docker Engine](https://docs.docker.com/install/)
* [Docker Compose](https://docs.docker.com/compose/install/)

Par défaut, notre stack expose les ports suivants :
* 3000 : NodeJS HTTP
* 8080 : NodeJS TCP Transport
* 27017 : TCP Input MongoDB

## Utilisation

### Déployer le stack

Cloner ce repository sur votre hôte Docker ou télécharger l'archive depuis le lien de la branche principale.
Ouvrer la console de votre choix et placer vous à la racine du projet.

```console
> docker-compose up
```

### Suppression

Pour stopper les services et supprimer tous les conteneurs, réseaux, volumes et images associés; exécuter la commande suivante :

```console
> docker-compose down -v
```

### Tester l'application

Pour vérifier que l'application Web est disponible et fonctionnelle, vous pouvez vous rendre sur les adresses suivantes :
* http://localhost:3000 : application de création de compte et d'envois de message (frontend)
* http://localhost:8080 : page par défaut de NodeJS (backend)
* http://localhost:27017 : page par défaut de MongoDB (backend)

## Configuration Docker

### Frontend

Voir les commentaires du Dockerfile dans le dossier /frontend.

### Backend

Voir les commentaires du Dockerfile dans le dossier /backend.

### docker-compose.yml

Voir les commentaires de docker-compose.yml à la racine du projet.

## Diagramme d'architecture (architecture.png)

Voir le fichier architecture.png à la racine du projet.