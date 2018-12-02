[:arrow_backward:](BRISTOL.md)

- [Les commandes](#les-commandes)
  - [Configuration de Git](#configuration-de-git)
  - [Création d'un projet](#creation-dun-projet)
  - [Projet existant](#projet-existant)
  - [Les commandes de base](#les-commandes-de-base)
  - [Les branches](#les-branches)


# Les commandes

## Configuration de Git

Si vous utilisez Git pour la première fois, vous aurez besoin de configurer vos informations utilisateur.

| Commandes                                | Description                          |
| ---------------------------------------- | ------------------------------------ |
| git config --global user.name "[nom]"    | Précise votre nom d'utilisateur      |
| git config --global user.email "[email]" | Précise votre email                  |

Ces informations seront ensuite disponible dans chaques commits.

![Exemple de commit](images/commit.png)

## Création d'un projet

Si vous êtes à l'origine du projet vous devez initialiser Git comme ceci:

| Commandes                                | Description                                   |
| ---------------------------------------- | ------------------------------------------------ |
| git init [nom]                           | Créer un dossier .git conservant l'historique    |
| git remote add [alias] [url]             | Fait un lien entre votre dossier local et disant |

## Projet existant

Lorsqu'un projet existe déjà, vous avez besoin de le cloner:

| Commandes                                | Description                                   |
| ---------------------------------------- | --------------------------------------------- |
| git clone [url]                          | Copie le projet dans votre dossier courant    |

Vous pouvez cloner en utilisant un lien HTTPS ou SSH. Pour utiliser une connexion SSH, il vous faut suivre [ce lien](https://help.github.com/articles/connecting-to-github-with-ssh/)

Dans le cas d'une connexion HTTPS vous aurez besoin d'entrer vos données de connexion à Github.

## Les commandes de base

| Commandes                                | Description                                    |
| ---------------------------------------- | --------------------------------------------------------- |
| git add [fichiers]                       | Sélectionne le.s fichier.s pour être versionné            |
| git add .                                | Sélectionne tous les fichiers versionnable                |
| git commit -m "description"              | Versionne les modifications en y associant un message  |
| git push                                 | Envoie les modifications vers le dépôt distant (github) |
| git pull                                 | Récupère les modifications depuis le dépôt distant  |

## Les branches

| Commandes                                | Description                                   |
| ---------------------------------------- | --------------------------------------------- |
| git branch [nom]                         | Créer une branche depuis la branche courante  |
| git checkout [nom]                       | Aller sur la branche specifié                 |
| git checkout -b [nom]                    | Fait les deux commandes précédentes           |