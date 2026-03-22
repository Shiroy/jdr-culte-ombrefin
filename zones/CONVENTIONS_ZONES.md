# Conventions — Structure des zones géographiques

## Règle fondamentale

La fiche d'une zone et le dossier de ses enfants sont **au même niveau**, et portent le **même nom** :

```
zones/
├─ CALEDONIE.md          ← fiche de la Calédonie
├─ CALEDONIE/            ← enfants de la Calédonie
│  ├─ VAL_DORE.md        ← fiche du Val-Doré
│  ├─ VAL_DORE/          ← enfants du Val-Doré
│  │  ├─ PONT_SUR_DOUVE.md     ← fiche de Pont-sur-Douve
│  │  ├─ PONT_SUR_DOUVE/       ← enfants de Pont-sur-Douve
│  │  │  ├─ CASERNE.md
```

## Règles de nommage

- Noms de fichiers et dossiers en **MAJUSCULES_AVEC_UNDERSCORES**
- Extension `.md` pour toutes les fiches

## Liens relatifs

Les liens entre fiches suivent naturellement cette structure :

| Depuis | Vers | Lien |
|--------|------|------|
| `CALEDONIE.md` | `CALEDONIE/VAL_DORE.md` (enfant) | `./CALEDONIE/VAL_DORE.md` |
| `CALEDONIE/VAL_DORE.md` | `CALEDONIE.md` (parent) | `../CALEDONIE.md` |
| `CALEDONIE/VAL_DORE.md` | `CALEDONIE/VAL_DORE/PONT_SUR_DOUVE.md` (enfant) | `./VAL_DORE/PONT_SUR_DOUVE.md` |
| `CALEDONIE/VAL_DORE/PONT_SUR_DOUVE.md` | `CALEDONIE/VAL_DORE.md` (parent) | `../VAL_DORE.md` |

## Métadonnées des fiches

Chaque fiche doit renseigner dans ses métadonnées :

- **Lieu parent** : lien vers la fiche du lieu parent (ou `_(racine — pas de fiche dédiée)_`)
- **Lieux enfants** : liens vers les fiches enfants directes
