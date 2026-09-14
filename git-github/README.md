# Audit des images — Git & GitHub

## Statut

Audit des références d'images présentes dans `index.html`.

### Problème identifié

Les captures du rapport sont bien présentes dans `git-github/assets/images/`, mais plusieurs références HTML utilisent `assets/images/...` depuis `git-github/index.html`.

Le chemin relatif correct vers ce dossier local est :

```text
assets/images/...        ❌ référence actuelle
../assets/images/...     ⚠️ seulement si l'image est dans le dossier global
./assets/images/...      ❌ ne correspond pas au dossier actuel
```

Pour les captures propres au rapport, le chemin attendu est :

```text
git-github/assets/images/<fichier>
```

et donc depuis `git-github/index.html` :

```html
<img src="assets/images/<fichier>">
```

Cette partie est donc à distinguer d'une image réellement absente : les fichiers locaux existent, mais certaines références ne pointent pas vers le bon emplacement selon l'organisation actuelle du dépôt.

## Images locales à contrôler

Les ressources suivantes existent dans `git-github/assets/images/` et doivent être comparées aux références du rapport :

- `git.webp`
- `github.png`
- `git_v_github.png`
- `git-site.png`
- `install git.png`
- `git version.png`
- `wml.png`
- `git config.png`
- `git init.png`
- `git add.png`
- `git branch.png`
- `git create repo.png`
- `git edit.png`
- `git login.png`
- `git new repo.png`
- `git push.png`
- `git remote.png`
- `git restatus.png`
- `git status.png`
- `github info.png`
- `github-git.png`
- `index-html.png`

## Action recommandée

1. Vérifier chaque `<img src="...">` de `index.html`.
2. Conserver les images propres au rapport dans `git-github/assets/images/`.
3. Utiliser les chemins relatifs correspondant réellement à l'emplacement du fichier HTML.
4. Ne pas créer de doublons dans `assets/images/` global uniquement pour masquer un mauvais chemin.

## Conclusion

**Images réellement absentes : non confirmées dans ce rapport.**

Le problème principal est une **incohérence de chemin**, à corriger lors de la passe de normalisation Git & GitHub.
