# Audit des images — AWS IAM

## Statut

Audit des références d'images de `aws/iam/index.html`.

## Images manquantes

Les deux références suivantes sont utilisées dans le rapport mais ne sont pas présentes dans `assets/images/` global :

| Référence HTML | État | Emplacement attendu |
|---|---|---|
| `../../assets/images/mfa-root.png` | ❌ Absente | `assets/images/mfa-root.png` |
| `../../assets/images/iam-users.png` | ❌ Absente | `assets/images/iam-users.png` |

### 1. `mfa-root.png`

**Utilisation :** illustration de la configuration MFA du compte racine AWS.

**À créer :** capture d'écran montrant l'étape pertinente de configuration/activation de la MFA du compte racine, sans exposer de données sensibles.

### 2. `iam-users.png`

**Utilisation :** illustration de la liste des utilisateurs IAM dans la console AWS.

**À créer :** capture d'écran de la page IAM Users, avec les éventuels noms, comptes ou identifiants sensibles masqués si nécessaire.

## Consigne de sécurité

Ne pas capturer dans les images :

- Access Keys ou Secret Access Keys ;
- mots de passe ;
- QR codes MFA ;
- tokens temporaires ;
- informations personnelles inutiles.

## Conclusion

**Images manquantes confirmées : 2.**
