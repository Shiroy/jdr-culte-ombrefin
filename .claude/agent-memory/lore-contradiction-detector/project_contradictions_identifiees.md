---
name: Contradictions et ambiguïtés identifiées — audit 2026-03-22
description: Résultat de l'audit complet du 2026-03-22 — contradictions identifiées, statut de résolution
type: project
---

## Audit effectué le 2026-03-22

### Renommage vérifié
La "Secte de Myrkul" a été correctement renommée en "Culte de l'Ombrefin" dans tous les fichiers. Aucune occurrence résiduelle de l'ancienne appellation. Myrkul subsiste uniquement comme nom de la divinité (légitime).

### Contradictions résolues

**Contradiction #1 — Accord grammatical** ✅ RÉSOLUE
**Contradiction #2 — Puissance des cités finoriennes** ✅ RÉSOLUE
**Contradiction #3 — Intensité de la crise royale** ✅ RÉSOLUE
**Contradiction #4 — Statut de manipulation des finoriens** ✅ RÉSOLUE
**Contradiction #5 — Noms du fleuve** ✅ COHÉRENTE
**Contradiction #6 — Hiérarchie géographique du Val-Doré** ✅ RÉSOLUE
**Contradiction terminologique — "Hameau" vs "Village"** ✅ RÉSOLUE
**Contradiction POI — "Place forte centrale" anonyme** ✅ RÉSOLUE
**Contradiction PNJ — Seigneur local anonyme** ✅ RÉSOLUE
**Contradiction T1 — Liens brisés dans MONDE.md** ✅ RÉSOLUE (2026-03-22)
**Contradiction T2 — Chemin relatif brisé dans zones/REGIONS_FINORIENNES.md** ✅ RÉSOLUE (2026-03-22)

---

### Ambiguïtés résolues (session 2026-03-22)

**Rumeur du marchand finorien (Hautefauche)** ✅ TRANCHÉE
- Décision : rumeur spontanée née de la peur et de la paranoïa collective. Pas de fondement réel, pas de manipulation du Culte.
- Marquée "(Faux)" dans HAUTEFAUCHE.md.

**Nobles conspirateurs au Val-Doré** ✅ TRANCHÉE
- Décision : seigneurs vassaux d'autres régions de Calédonie qui convoitent le Val-Doré pour son poids économique et son levier vers le trône. Pas d'agents infiltrés sur place.
- Documenté dans faction/NOBLES_CONSPIRATEURS.md.

**Nom neutre du fleuve** ✅ TRANCHÉ
- Décision : **L'Aevyne** — nom diplomatique bilatéral utilisé dans les traités et textes officiels.
- Documenté dans MONDE.md (présentation).

**Distance Hautefauche — Pont-sur-Douve** ✅ TRANCHÉE
- Décision : une journée de voyage.
- Mis à jour dans HAUTEFAUCHE.md (identité + localisation) et VAL_DORE.md (POI Hautefauche).

---

### Ambiguïtés toujours ouvertes (non bloquantes)

**Ambiguïté — Nom du continent**
- Décision reportée : inutile pour l'instant, à nommer quand un texte in-world l'exigera.

**Ambiguïté — Marchands finoriens**
- Décision reportée : statut (passif ou actif) à définir selon les besoins scénaristiques.

**Ambiguïté — Étymologie de "Ombrefin"**
- Volontairement mystérieux. L'auteur se réserve la possibilité de définir l'étymologie plus tard.

**Ambiguïté — Distances entre autres localités du Val-Doré**
- À établir par un tableau dans VAL_DORE.md quand 2-3 villages supplémentaires auront été créés.

---

### Audit PNJ EDOUARD_DE_CHAMP_D_OR — 2026-03-22

**Contradiction L1 — Lien brisé vers Pont-sur-Douve (section "Zone(s) de présence")** — OUVERTE
- Ligne 162 de la fiche PNJ : `../PONT_SUR_DOUVE.md`
- Depuis `zones/CALEDONIE/VAL_DORE/PONT_SUR_DOUVE/PNJ/`, ce chemin pointe vers `zones/CALEDONIE/VAL_DORE/PONT_SUR_DOUVE/PONT_SUR_DOUVE.md` qui n'existe pas.
- Fichier réel : `zones/CALEDONIE/VAL_DORE/PONT_SUR_DOUVE.md`
- Correction : remplacer `../PONT_SUR_DOUVE.md` par `../../PONT_SUR_DOUVE.md`

**Contradiction L2 — Lien brisé vers Val-Doré (section "Zone(s) de présence")** — OUVERTE
- Ligne 162 de la fiche PNJ : `../../VAL_DORE.md`
- Depuis `zones/CALEDONIE/VAL_DORE/PONT_SUR_DOUVE/PNJ/`, ce chemin pointe vers `zones/CALEDONIE/VAL_DORE/VAL_DORE.md` qui n'existe pas.
- Fichier réel : `zones/CALEDONIE/VAL_DORE.md`
- Correction : remplacer `../../VAL_DORE.md` par `../../../VAL_DORE.md`

**Contradiction L3 — Deux chemins contradictoires vers faction/ROYAUME_CALEDONIE.md** — OUVERTE
- Ligne 104 (section "Appartenance") : `../../../../faction/ROYAUME_CALEDONIE.md` — incorrect (remonte à `zones/faction/` inexistant)
- Ligne 163 (section "Liens") : `../../../../../faction/ROYAUME_CALEDONIE.md` — correct (remonte à la racine puis `faction/`)
- Correction : ligne 104, remplacer `../../../../faction/ROYAUME_CALEDONIE.md` par `../../../../../faction/ROYAUME_CALEDONIE.md`

**Why:** Résultats d'audit, utiles pour les corrections futures et pour éviter de signaler les mêmes problèmes deux fois.
**How to apply:** Vérifier le statut de ces points avant chaque nouvel audit. Mettre à jour ce fichier si l'auteur confirme une résolution.
