# Registre de preuve de covoiturage

Site vitrine du Registre. https://covoiturage.beta.gouv.fr

-

## Mises à jour

### Ajouter un opérateur ou un territoire

1. Dans le dossier `content/operateurs` ou `content/territoires`, dupliquer un fichier `.md` existant et modifier sa date de création dans l'en-tête du fichier.
2. Uploader le logo dans `static/operateurs` et `static/territoires` et configurer le nom dans le fichier `.md` précédemment créé. Une taille de 480x480 est suffisante.
3. Commiter les modifications

#### Opérateur

```markdown
---
title: "Maxicovoit"
date: 2020-12-28T15:46:34Z
logo: maxicovoit.png
---
```

#### Territoire

```markdown
---
title: "Communauté d'Agglomération des dieux de l'Olympe"
date: 2020-12-28T15:46:34Z
showTitle: true # option nécessaire pour afficher le nom du territoire
logo: olympus.png
---
```

## Tech

Le site utilise le générateur de sites statiques [HUGO](https://gohugo.io/).
L'installation en local utilise Docker et Docker Compose.

### Installation

Cloner le dépôt et lancer la commande de développement.

### Développement

```shell
docker-compose up server
```

http://localhost:1313/

### Déploiement

```shell
docker-compose run hugo -e production
rsync -avz public/* rpc:www/home/
```

# License

DINUM, 2020-2021.

The source code is published under [Apache license 2.0](https://github.com/betagouv/preuve-covoiturage-vitrine/blob/main/LICENSE).
