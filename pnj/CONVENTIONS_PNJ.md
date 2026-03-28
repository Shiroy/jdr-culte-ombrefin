# Conventions — Structure des PNJs

## Règle fondamentale

Toutes les fiches PNJ sont centralisées dans le dossier **`pnj/`** à la racine du projet, quelle que soit la zone géographique de rattachement du personnage.

```
pnj/
├─ CONVENTIONS_PNJ.md
├─ ARMAND_LEFEBVRE.md
├─ EDOUARD_DE_CHAMP_D_OR.md
├─ ALDREN_MAISON_LUMINIS.md
├─ ...
```

## Règles de nommage

- Noms de fichiers en **MAJUSCULES_AVEC_UNDERSCORES**
- Utiliser le nom le plus connu du PNJ (surnom inclus si c'est son identifiant principal)
- Extension `.md` pour toutes les fiches

## Zone de rattachement

La zone de rattachement d'un PNJ est documentée dans les **métadonnées de la fiche** (champ `Zone(s) de présence`), pas dans la structure de dossiers.

## Liens relatifs

| Depuis | Vers | Lien |
|--------|------|------|
| `pnj/ARMAND_LEFEBVRE.md` | zone de présence | `../zones/CALEDONIE/VAL_DORE/HAUTEFAUCHE.md` |
| `zones/CALEDONIE/VAL_DORE/HAUTEFAUCHE.md` | PNJ de la zone | `../../pnj/ARMAND_LEFEBVRE.md` |
| `campagne/mon-aventure/cadre.md` | fiche PNJ | `../../pnj/ARMAND_LEFEBVRE.md` |

## Métadonnées des fiches

Chaque fiche PNJ doit renseigner dans ses métadonnées :

- **Zone(s) de présence** : lien vers la fiche de zone de rattachement
- **PNJ liés** : liens vers les fiches des PNJs avec qui il a des relations notables
- **Faction(s)** : liens vers les fiches de factions concernées
