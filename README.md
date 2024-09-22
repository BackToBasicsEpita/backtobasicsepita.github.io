# Site web pour BackToBasics

## Prérequis

Avant de commencer, assurez-vous d'avoir les outils suivants installés sur votre machine, si vous utilisez **Nix** vous avez un [flake.nix](flake.nix):

- [Go](https://go.dev/) (minimum version v1.20)
- [Hugo Extended](https://gohugo.io/) (minimum version: 0.120.0)

## Installation

Clonez le repository du projet :

```sh
   git clone git@github.com:BackToBasicsEpita/backtobasicsepita.github.io.git
   cd site
```

## Développement

Pour lancer le serveur de développement et voir votre site en local :

```sh
    hugo server -D
```

Le site sera disponible à l'adresse : [http://localhost:1313](http://localhost:1313).

## Créer un sujet:

Pour créer un sujet vous aurez la documentation complète sur le site en local [localhost:1313/docs](https://localhost:1313/docs)

Si votre chapitre n'est pas disponible, vous devrez faire :
```sh
hugo -k new chapitre path/to/your/chapitre
```

Sinon/Puis :

```sh
hugo -k new cours path/to/your/course/name
```

## Comment soummettre ma fiche ?

- **Créer une branche pseudo/cours**
- **Faire une pull request**
- **Demander à ce que votre branch soit review et attendre qu'elle soit merge par un membre du bureau**
