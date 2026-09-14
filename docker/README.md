# Audit des images — Docker

## Statut

Audit des références d'images de `docker/index.html`.

## Résultat

Aucune image réellement absente n'a été identifiée parmi les références contrôlées.

Les ressources du rapport sont stockées dans :

```text
docker/assets/images/
```

Les références du fichier HTML utilisent le chemin relatif :

```text
assets/images/...
```

Ce chemin est cohérent avec l'emplacement de `docker/index.html`.

## Images contrôlées

Les références rencontrées correspondent notamment à :

- `docker.png`
- `prepare.png`
- `install.png`
- `start.png`
- `group.png`
- `run.png`
- `web-nginx.png`
- `welcome-nginx.png`
- `alpine.png`
- `tar.png`
- `login.png`
- `login-success.png`
- `reseau.png`
- `version.png`
- `hello.png`

Ces fichiers sont présents dans le dossier d'images Docker.

## Conclusion

**Images manquantes : aucune confirmée.**

Le rapport Docker reste volontairement hors du chantier de correction technique principal pour le moment.
