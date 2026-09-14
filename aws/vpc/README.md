# Audit des images — AWS VPC

## Statut

Audit des références d'images de `aws/vpc/index.html`.

## Images manquantes

Les références suivantes sont utilisées dans le rapport mais les fichiers correspondants ne sont pas présents dans `assets/images/` global :

| Référence HTML | État | Emplacement attendu |
|---|---|---|
| `../../assets/images/vpc-diagram.png` | ❌ Absente | `assets/images/vpc-diagram.png` |
| `../../assets/images/route-tables.png` | ❌ Absente | `assets/images/route-tables.png` |

### 1. `vpc-diagram.png`

**Utilisation :** illustration de la topologie VPC avec sous-réseaux publics et privés.

**À créer :** schéma ou capture de l'architecture comprenant VPC, Availability Zones, subnets publics/privés, Internet Gateway et NAT Gateway.

### 2. `route-tables.png`

**Utilisation :** illustration des tables de routage du VPC.

**À créer :** capture ou schéma montrant les associations des subnets et les routes par défaut vers l'Internet Gateway ou le NAT Gateway.

## Consigne de sécurité

Les captures de console AWS doivent éviter d'exposer des informations de compte ou des données sensibles inutiles.

## Conclusion

**Images manquantes confirmées : 2.**
