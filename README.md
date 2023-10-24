# Registre de preuve de covoiturage

Site vitrine du Registre. https://covoiturage.beta.gouv.fr

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

# Edition du site

Le site est déprécié et l'interface d'administration a été supprimée. Les modifications sont à faire à la main.

## Ajouter un opérateur

1. Ajouter le logo en `.webp/.png/.jpg` dans `src/static/images/operateurs/`
2. Dupliquer un fichier `content/operateurs/` et le modifier

# License

DINUM, 2020-2023.

The source code is published under [Apache license 2.0](https://github.com/betagouv/preuve-covoiturage-vitrine/blob/main/LICENSE).
