# Conventions — Structure des PNJs

## Règle fondamentale

Les PNJs sont **co-localisés avec leur zone** : les fiches de personnages présents dans une zone se trouvent dans un sous-dossier `PNJ/` à l'intérieur du dossier enfant de cette zone.

```
zones/
├─ CALEDONIE.md
├─ CALEDONIE/
│  ├─ VAL_DORE.md
│  ├─ VAL_DORE/
│  │  ├─ PONT_SUR_DOUVE.md
│  │  ├─ PONT_SUR_DOUVE/
│  │  │  ├─ PNJ/
│  │  │  │  ├─ ALDRIC_FERRANT.md    ← PNJ présent à Pont-sur-Douve
│  │  │  │  ├─ MIRA_LA_BOITEUSE.md
│  │  ├─ PNJ/
│  │  │  ├─ COMTE_EDRAN.md          ← PNJ à l'échelle du Val-Doré
```

## Règles de nommage

- Noms de fichiers en **MAJUSCULES_AVEC_UNDERSCORES**
- Utiliser le nom le plus connu du PNJ (surnom inclus si c'est son identifiant principal)
- Extension `.md` pour toutes les fiches

## Zone de rattachement

Un PNJ est rattaché à la **zone la plus précise** où il est habituellement présent :
- Un garde de la caserne → dans `PONT_SUR_DOUVE/PNJ/`
- Un noble qui gouverne le Val-Doré → dans `VAL_DORE/PNJ/`
- Un archimage itinérant à l'échelle de la Calédonie → dans `CALEDONIE/PNJ/`

## PNJs sans ancrage géographique fixe

Les PNJs itinérants ou à portée mondiale sont rangés dans :

```
pnj/
├─ CONVENTIONS_PNJ.md
├─ PNJ_ITINERANTS/
│  ├─ NOM_DU_PNJ.md
```

## Liens relatifs

| Depuis | Vers | Lien |
|--------|------|------|
| `VAL_DORE/PNJ/COMTE_EDRAN.md` | zone de présence | `../VAL_DORE.md` |
| `VAL_DORE.md` | PNJ de la zone | `./VAL_DORE/PNJ/COMTE_EDRAN.md` |
| `VAL_DORE/PNJ/COMTE_EDRAN.md` | autre PNJ de la même zone | `./MIRA_LA_BOITEUSE.md` |

## Métadonnées des fiches

Chaque fiche PNJ doit renseigner dans ses métadonnées :

- **Zone(s) de présence** : lien vers la fiche de zone de rattachement
- **PNJ liés** : liens vers les fiches des PNJs avec qui il a des relations notables
- **Faction(s)** : liens vers les fiches de factions concernées
