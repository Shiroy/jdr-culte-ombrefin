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

**Contradiction L1 — Lien brisé vers Pont-sur-Douve (section "Zone(s) de présence")** ✅ RÉSOLUE (2026-03-22)
- Corrigé : `../PONT_SUR_DOUVE.md` → `../../../PONT_SUR_DOUVE.md`

**Contradiction L2 — Lien brisé vers Val-Doré (section "Zone(s) de présence")** ✅ RÉSOLUE (2026-03-22)
- Corrigé : `../../VAL_DORE.md` → `../../../../VAL_DORE.md`

**Contradiction L3 — Deux chemins contradictoires vers faction/ROYAUME_CALEDONIE.md** ✅ RÉSOLUE (vérification 2026-03-22)
- Ligne 104 déjà correcte dans le fichier (`../../../../../faction/ROYAUME_CALEDONIE.md`). La contradiction signalée ne correspondait plus à l'état réel du fichier.

---

### Audit ciblé — Gentilé "Haut-Faucheur / Haute-Faucheuse" — 2026-03-22

**Résultat : AUCUNE CONTRADICTION INTRODUITE**

- Le gentilé n'apparaît que dans `HAUTEFAUCHE.md` (ligne 17) — aucun conflit textuel avec aucun autre fichier.
- Morphologie cohérente avec le nom du lieu et le registre linguistique de l'univers.
- Observation structurelle : le champ "Gentilé" n'existe pas dans le template `make-zone/zone_template.md`. Recommandation : l'y ajouter entre "Surnoms & noms locaux" et "Localisation".
- Lacune résiduelle non bloquante : Pont-sur-Douve n'a pas encore de gentilé.

---

### Audit PNJ ARMAND_LEFEBVRE — 2026-03-22

**Résultat : AUCUNE CONTRADICTION DÉTECTÉE**

Cohérence vérifiée sur les points suivants :
- Lien faction `../../../../../faction/ROYAUME_CALEDONIE.md` : correct (remonte à la racine depuis `HAUTEFAUCHE/PNJ/`)
- Lien zone `../../HAUTEFAUCHE.md` : correct
- Affiliation "Comté du Val-Doré, Royaume de Calédonie" : cohérent avec MONDE.md et faction/ROYAUME_CALEDONIE.md
- Épidémie liée au Culte de l'Ombrefin (section Aspects magiques) : cohérent avec CULTE_OMBREFIN.md
- Comte Édouard de Champ-d'Or mentionné indirectement (Armand est "sous l'autorité du Comté du Val-Doré, loyal au Comte Édouard de Champ-d'Or") : cohérent avec EDOUARD_DE_CHAMP_D_OR.md
- Population 150 habitants : conforme aux données de référence établies par HAUTEFAUCHE.md
- Chauntea comme divinité du village : conforme au canon (Chauntea = divinité populaire calédonienne)
- Culte de l'Ombrefin absent de la fiche faction d'Armand (il n'en fait pas partie) : correct
- Ton et ambiance (thriller rural pastoral) : cohérent avec VAL_DORE.md et HAUTEFAUCHE.md

**Convention narrative confirmée (2026-03-22)** :
- "Aventuriers" et "soldats mandatés par le Comte" sont des termes interchangeables pour désigner les joueurs. Ce n'est pas une ambiguïté de lore. Ne plus signaler ce point dans les audits futurs.

**Why:** Résultats d'audit, utiles pour les corrections futures et pour éviter de signaler les mêmes problèmes deux fois.
**How to apply:** Vérifier le statut de ces points avant chaque nouvel audit. Mettre à jour ce fichier si l'auteur confirme une résolution.

---

### Audit CASERNE.md — 2026-03-22

**Résultat : AUCUNE CONTRADICTION DÉTECTÉE**

Cohérence vérifiée sur les points suivants :
- Effectif garnison 150-200 soldats : cohérent avec PONT_SUR_DOUVE.md (ligne 69)
- Lieu parent Pont-sur-Douve, lien `../PONT_SUR_DOUVE.md` : correct depuis `PONT_SUR_DOUVE/`
- Lien faction `../../../../faction/ROYAUME_CALEDONIE.md` : correct (4 niveaux depuis `PONT_SUR_DOUVE/`)
- PNJ Édouard de Champ-d'Or comme commanditaire ultime : cohérent avec EDOUARD_DE_CHAMP_D_OR.md et cadre.md
- Lien `./PNJ/EDOUARD_DE_CHAMP_D_OR.md` et `./PNJ/GILLES_DE_MARNAC.md` : cohérents avec la structure du dossier
- Tyr mentionné (amulettes personnelles) : cohérent avec la chapelle Tyr du château-comtal dans PONT_SUR_DOUVE.md
- Gilles de Marnac (nouveau PNJ) : non mentionné ailleurs, pas de conflit — fiche à créer ultérieurement
- PONT_SUR_DOUVE.md mis à jour (lieux enfants) : lien `./PONT_SUR_DOUVE/CASERNE.md` correct
- Lacune résiduelle non bloquante : Gilles de Marnac n'a pas encore de fiche PNJ dédiée (signalé dans les liens de CASERNE.md)

---

### Audit PNJ ALDREN_MAISON_LUMINIS — 2026-03-23

**Résultat : AUCUNE CONTRADICTION DE LORE — 3 erreurs de chemins relatifs à corriger**

Cohérence de lore vérifiée sur les points suivants :
- Race humain, origine finorienne : cohérent (VAL_DORE.md mentionne "Marchands finoriens — Diverses races")
- Maison marchande mineure dans une magocratie : cohérent et bien exploité narrativement (REGIONS_FINORIENNES.md)
- Renégociation commerciale dans l'instabilité calédonienne : cohérent avec REGIONS_FINORIENNES.md ("certaines cités cherchent à renégocier les termes commerciaux")
- Présence sur la route commerciale du Val-Doré : cohérent (VAL_DORE.md confirme la présence de marchands finoriens)
- Rôle de fausse piste épidémie Hautefauche : cohérent avec HAUTEFAUCHE.md (rumeur "(Faux)" déjà établie)
- Indépendance politique vis-à-vis des cités-états : cohérent avec la structure fédérale lâche de REGIONS_FINORIENNES.md
- Bienfaiteur anonyme (dette) : volontairement non défini, aucun conflit possible

**Erreurs de chemins relatifs (non bloquantes pour le lore) :**
- `../VAL_DORE/HAUTEFAUCHE.md` → doit être `../HAUTEFAUCHE.md` (depuis `VAL_DORE/PNJ/`)
- `../VAL_DORE.md` → doit être `../../VAL_DORE.md`
- `../../../faction/REGIONS_FINORIENNES.md` → doit être `../../../../faction/REGIONS_FINORIENNES.md`

**Pattern récurrent confirmé** : les erreurs de profondeur de chemins relatifs dans les fiches PNJ sont un défaut structurel récurrent (déjà identifié sur EDOUARD_DE_CHAMP_D_OR, ARMAND_LEFEBVRE). Les PNJ dans `VAL_DORE/PNJ/` sont à 4 niveaux de profondeur depuis la racine : `../../../../` pour atteindre `faction/`.
