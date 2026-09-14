# Audit des images — AWS Linux Web Server

## Statut

Audit des références d'images de `aws/linux-webserver/index.html`.

## Images manquantes

Les références suivantes sont présentes dans le rapport mais les fichiers correspondants ne sont pas présents dans le dossier global `assets/images/` :

| Référence HTML | État | Emplacement attendu |
|---|---|---|
| `../../assets/images/ec2-launch.png` | ❌ Absente | `assets/images/ec2-launch.png` |
| `../../assets/images/apache-installed.png` | ❌ Absente | `assets/images/apache-installed.png` |
| `../../assets/images/browser-test.png` | ❌ Absente | `assets/images/browser-test.png` |

### 1. `ec2-launch.png`

**Utilisation :** écran de lancement/configuration d'une instance EC2 Linux.

**À créer :** capture de la configuration EC2 utilisée pour le TP, sans exposer de données sensibles.

### 2. `apache-installed.png`

**Utilisation :** preuve de l'installation et du démarrage d'Apache (`httpd`) sur Amazon Linux 2023.

**À créer :** capture du terminal montrant les commandes d'installation et/ou `systemctl status httpd`.

### 3. `browser-test.png`

**Utilisation :** validation de l'accès au serveur Web depuis un navigateur.

**À créer :** capture de la page Web déployée, idéalement avec l'adresse publique partiellement masquée si nécessaire.

## Consigne de sécurité

Éviter d'afficher dans les captures : clés privées, informations AWS sensibles, identifiants personnels ou données de connexion.

## Conclusion

**Images manquantes confirmées : 3.**
