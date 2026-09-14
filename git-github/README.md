# Audit des images — Git & GitHub

## Statut

Audit des références d'images présentes dans `git-github/index.html`.

## Résultat

Aucune image réellement absente n'a été confirmée.

Les captures propres au rapport sont stockées dans :

```text
git-github/assets/images/
```

Depuis `git-github/index.html`, une référence telle que :

```html
<img src="assets/images/git.webp">
```

est correcte, car elle pointe vers `git-github/assets/images/git.webp`.

Les images communes de la page de garde utilisent quant à elles :

```html
<img src="../assets/images/senegal-flag.png">
<img src="../assets/images/udb.jpeg">
```

ce qui est également correct.

## Images locales contrôlées

Les ressources présentes dans `git-github/assets/images/` comprennent notamment :

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

## Conclusion

**Images manquantes confirmées : aucune.**

Aucune création d'image n'est donc nécessaire pour ce rapport dans le cadre de cet audit.
