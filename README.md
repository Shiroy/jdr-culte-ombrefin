# Les Comtes de l'Ombrefin — Guide du Maître de Jeu

Bienvenue dans **Les Comtes de l'Ombrefin**, une campagne D&D 5e se déroulant sur un continent de médiéval-fantasy déchiré par des tensions politiques et une menace secrète. Ce guide vous permet de vous orienter dans les fichiers du projet avant de mener votre première session.

---

## Le monde en un coup d'œil

Deux grandes puissances s'affrontent — sans encore se faire la guerre :

- **La Calédonie** à l'ouest : un royaume féodal classique, en pleine crise politique. Le roi a tenté un rapprochement avec les cités finoriennes, s'attirant l'hostilité d'une noblesse conservatrice qui conspire dans son dos.
- **Les Régions finoriennes (Finoryn)** à l'est : une fédération de cités-états gouvernées par des mages. Technologiquement et magiquement avancées, elles entretiennent avec la Calédonie une relation commerciale vitale — et un mépris mutuel à peine dissimulé.

Les deux nations sont séparées par un grand fleuve (**la Veyne** côté calédonien, l'**Aethros** côté finorien, l'**Aevyne** dans les traités), franchissable en quelques postes-frontières gardés.

**Dans l'ombre**, le **Culte de l'Ombrefin** — des mages renégats et des calédoniens corrompus vénérant une cabale de cinq dieux mineurs — orchestre patiemment une guerre entre les deux nations. Leur objectif : des millions de morts pour hisser leurs divinités au rang de puissances majeures.

> Pour commencer, lire : [MONDE.md](./MONDE.md)

---

## La campagne en cours : *Le Mal de Hautefauche*

**Niveau 3 — 3 à 4 sessions**

Le village d'Hautefauche est frappé par une épidémie mystérieuse. Une rumeur enfle : un marchand finorien en serait responsable. En réalité, une cellule du Culte de l'Ombrefin — dédiée à **Valtar, le Seigneur de la Peste** — a délibérément provoqué l'épidémie pour attiser la méfiance envers Finoryn.

Les joueurs, membres de la garnison de Pont-sur-Douve, sont mandatés discrètement par le Comte Édouard de Champ-d'Or pour enquêter.

> Cadre complet : [campagne/le-mal-de-hautefauche/cadre.md](./campagne/le-mal-de-hautefauche/cadre.md)

---

## Comment naviguer dans les fichiers

```
les-comtes-de-lombrefin/
├─ MONDE.md                          ← point d'entrée du lore global
├─ campagne/                         ← aventures jouables
│   └─ le-mal-de-hautefauche/
│       ├─ cadre.md                  ← structure narrative complète de l'aventure
│       ├─ cellule-valtar.md         ← la cellule antagoniste et son chef
│       └─ scenes/                   ← scènes prêtes à jouer (textes MJ)
├─ zones/                            ← géographie et lieux
│   ├─ CALEDONIE.md
│   └─ CALEDONIE/
│       └─ VAL_DORE/
│           ├─ PONT_SUR_DOUVE.md     ← quartier général du Comte
│           ├─ HAUTEFAUCHE.md        ← théâtre de l'enquête
│           └─ PONT_SUR_DOUVE/
│               └─ CASERNE.md        ← lieu du briefing initial
├─ faction/                          ← factions politiques et secrètes
│   ├─ CULTE_OMBREFIN.md            ← antagoniste principal de la campagne
│   ├─ ASSEMBLEE_DERNIER_SOUFFLE.md ← les cinq dieux du culte
│   ├─ ROYAUME_CALEDONIE.md
│   ├─ REGIONS_FINORIENNES.md
│   └─ NOBLES_CONSPIRATEURS.md
├─ pnj/                              ← fiches personnages (tous centralisés ici)
│   ├─ EDOUARD_DE_CHAMP_D_OR.md     ← commanditaire
│   ├─ ARMAND_LEFEBVRE.md           ← bailli de Hautefauche
│   ├─ ALDREN_MAISON_LUMINIS.md     ← marchand finorien, source d'info
│   └─ THOMIN_BEAUFORT.md
└─ objets/                           ← artefacts et objets notables
    ├─ MIROIRS_DE_MURMURE.md         ← artefacts de communication du culte
    └─ DECOUSEURS.md
```

---

## Préparer une session

### Ordre de lecture recommandé

1. **[MONDE.md](./MONDE.md)** — vue d'ensemble du monde, histoire, géographie, factions
2. **[faction/CULTE_OMBREFIN.md](./faction/CULTE_OMBREFIN.md)** — comprendre l'antagoniste, ses dieux, sa structure et ses méthodes
3. **[campagne/le-mal-de-hautefauche/cadre.md](./campagne/le-mal-de-hautefauche/cadre.md)** — structure narrative de l'aventure, PNJ clés, lieux, fins possibles
4. **Fiches de lieux** dans `zones/CALEDONIE/VAL_DORE/` — les zones traversées pendant l'aventure
5. **Fiches PNJ** dans `pnj/` — personnages avec qui les joueurs interagiront

### Scènes prêtes à jouer

Chaque scène contient un texte narratif lisible à voix haute et des notes MJ. Elles sont dans `campagne/le-mal-de-hautefauche/scenes/` :

| Scène | Résumé |
|-------|--------|
| [introduction/scene.md](./campagne/le-mal-de-hautefauche/scenes/introduction/scene.md) | Briefing à la caserne — ordre de mission donné par Gilles de Marnac |
| [pont-sur-douve-avant-depart/scene.md](./campagne/le-mal-de-hautefauche/scenes/pont-sur-douve-avant-depart/scene.md) | Fenêtre libre à Pont-sur-Douve avant le départ |
| [rencontre-aldren/scene.md](./campagne/le-mal-de-hautefauche/scenes/rencontre-aldren/scene.md) | Rencontre avec le marchand finorien Aldren sur la route |

---

## Les aides disponibles

### Claude comme co-MJ

Ce projet est conçu pour fonctionner avec Claude. Plusieurs skills sont disponibles pour enrichir le monde en cours de préparation :

| Commande | Usage |
|----------|-------|
| `/make-pnj` | Créer ou étoffer une fiche PNJ |
| `/make-zone` | Créer ou compléter une fiche de lieu |
| `/make-scene` | Rédiger une scène jouable |
| `/make-objet` | Créer un artefact ou objet notable |
| `/make-aventure` | Cadrer une nouvelle aventure |
| `/make-intrigue` | Structurer une intrigue dans une aventure |
| `/grill-me` | Approfondir un élément de lore (faction, magie, histoire…) |
| `/lore-contradiction-detector` | Auditer la cohérence du monde après un ajout |

### Conventions de structure

Chaque type de contenu a ses propres conventions documentées :

- PNJ : [pnj/CONVENTIONS_PNJ.md](./pnj/CONVENTIONS_PNJ.md)
- Zones : [zones/CONVENTIONS_ZONES.md](./zones/CONVENTIONS_ZONES.md)
- Objets : [objets/CONVENTIONS_OBJETS.md](./objets/CONVENTIONS_OBJETS.md)

---

## Contexte des joueurs

Les personnages joueurs sont des **soldats de la garnison de Pont-sur-Douve**, au service du Comte Édouard de Champ-d'Or. Ils ne sont pas encore des aventuriers itinérants — ce sont des gens du Val-Doré, enracinés localement, qui découvriront progressivement l'existence du Culte de l'Ombrefin. L'aventure *Le Mal de Hautefauche* est conçue pour être leur point d'entrée dans une campagne bien plus large.

---

*Système de jeu : D&D 5e*
