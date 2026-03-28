# Conventions — Structure des Objets

## Règle fondamentale

Toutes les fiches d'objets notables (artefacts, reliques, objets magiques, équipements emblématiques) sont centralisées dans le dossier **`objets/`** à la racine du projet.

```
objets/
├─ CONVENTIONS_OBJETS.md
├─ MIROIRS_DE_MURMURE.md
├─ ...
```

## Règles de nommage

- Noms de fichiers en **MAJUSCULES_AVEC_UNDERSCORES**
- Utiliser le nom le plus connu de l'objet (y compris le surnom s'il est l'identifiant principal)
- Extension `.md` pour toutes les fiches

## Ce qui appartient ici

- Artefacts magiques nommés ayant un rôle narratif
- Reliques liées à des factions ou événements historiques
- Équipements emblématiques associés à des PNJs importants
- Tout objet dont la description dépasse quelques lignes dans une autre fiche

## Ce qui n'appartient pas ici

- Équipements génériques sans identité propre (une épée ordinaire, une bourse de pièces)
- Objets d'aventure purement mécaniques sans ancrage dans le lore (à mettre dans la scène ou l'intrigue concernée)

## Métadonnées des fiches

Chaque fiche d'objet doit renseigner dans ses métadonnées :

- **Faction(s) liée(s)** : liens vers les fiches de factions concernées
- **PNJ lié(s)** : liens vers les fiches des PNJs associés
- **Zone(s) connue(s)** : lieux où l'objet a été vu ou utilisé

## Liens relatifs

| Depuis | Vers | Lien |
|--------|------|------|
| `objets/MIROIRS_DE_MURMURE.md` | faction liée | `../faction/CULTE_OMBREFIN.md` |
| `faction/CULTE_OMBREFIN.md` | objet | `../objets/MIROIRS_DE_MURMURE.md` |
| `campagne/mon-aventure/cadre.md` | objet | `../../objets/MIROIRS_DE_MURMURE.md` |
