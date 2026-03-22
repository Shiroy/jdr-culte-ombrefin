---
name: Contradictions et ambiguïtés identifiées — audit 2026-03-22
description: Résultat de l'audit complet du 2026-03-22 — contradictions identifiées, statut de résolution
type: project
---

## Audit effectué le 2026-03-22

### Renommage vérifié
La "Secte de Myrkul" a été correctement renommée en "Culte de l'Ombrefin" dans tous les fichiers. Aucune occurrence résiduelle de l'ancienne appellation. Myrkul subsiste uniquement comme nom de la divinité (légitime).

### Contradictions résolues (session de correction 2026-03-22)

**Contradiction #1 — Accord grammatical** ✅ RÉSOLUE
- Fichier : `faction/CULTE_OMBREFIN.md` ligne 27
- Déjà corrigée avant la session (probablement lors du commit Finoryn). Le fichier contenait déjà "calédoniennes".

**Contradiction #2 — Puissance des cités finoriennes** ✅ RÉSOLUE
- Fichier : `zones/REGIONS_FINORIENNES.md` ligne 15
- Ancienne formulation : "chaque cité est plus puissante que le royaume de Calédonie"
- Nouvelle formulation : "chaque cité dispose d'une supériorité magique et économique sur le royaume de Calédonie, mais leur fragmentation les prive de toute force militaire coordonnée"
- Justification : précise la nature de la supériorité (magique/économique) sans invalider la guerre ancienne conclue par "épuisement mutuel"

**Contradiction #3 — Intensité de la crise royale** ✅ RÉSOLUE
- Fichier : `zones/CALEDONIE.md` ligne 16
- Ancienne formulation : "créant un vide de pouvoir et une compétition ouverte"
- Nouvelle formulation : "leur succès, partiel mais réel, a fragilisé l'autorité royale et ouvert une compétition ouverte entre seigneurs vassaux"
- Aligné sur l'introduction_joueurs.md ("succès partiel, mais réel")

**Contradiction #4 — Statut de manipulation des finoriens** ✅ RÉSOLUE
- Fichier : `faction/REGIONS_FINORIENNES.md` ligne 26
- Ancienne formulation : "cible potentielle de manipulation"
- Nouvelle formulation : "déjà instrumentalisées à leur insu, poussées à réagir aux provocations fabriquées de toutes pièces"
- Aligné sur CULTE_OMBREFIN.md qui les décrit déjà comme "manipulées"

**Contradiction #5 — Noms du fleuve** ✅ VÉRIFIÉE COHÉRENTE
- Les deux noms (Veyne / Aethros) sont cohérents dans tous les fichiers. Pas de contradiction.

**Contradiction #6 — Hiérarchie géographique du Val-Doré** ✅ RÉSOLUE
- Fichier : `MONDE.md` section géographie
- Val-Doré était listé au même niveau que Calédonie et les Régions finoriennes
- Nouvelle présentation : Val-Doré indenté sous Calédonie avec annotation "sous-région agricole de Calédonie"

### Ambiguïtés en suspens (non bloquantes)

**Ambiguïté #1 — Étymologie de "Ombrefin"**
- Fichier : `faction/CULTE_OMBREFIN.md`
- Le nom "Ombrefin" n'est jamais expliqué. Risque si des fichiers futurs l'utilisent dans un autre sens.
- Priorité : faible, à traiter si le lore s'enrichit du côté religieux/cultiste

**Ambiguïté #3 — Nom neutre du fleuve**
- Le fleuve a deux noms (Veyne / Aethros) selon le côté. Aucun nom neutre pour les contextes diplomatiques officiels.
- Priorité faible jusqu'à l'introduction de documents bilatéraux.

**Ambiguïté #4 — Nom du continent**
- Le continent n'est nommé dans aucun fichier. Lacune à combler avant l'introduction de textes in-world.
- Priorité faible mais à surveiller.

### Vérification 2026-03-22 (audit "Finoryn")
Ajout du nom canonique "Finoryn" dans MONDE.md, zones/REGIONS_FINORIENNES.md, faction/REGIONS_FINORIENNES.md, campagne/introduction_joueurs.md. **Aucune nouvelle contradiction introduite.** Les fichiers non modifiés (CALEDONIE.md, VAL_DORE.md, CULTE_OMBREFIN.md, NOBLES_CONSPIRATEURS.md, ROYAUME_CALEDONIE.md) utilisent "Régions finoriennes" ou "cités finoriennes", ce qui est canoniquement correct selon la règle de nommage établie.

**Why:** Résultats d'audit, utiles pour les corrections futures et pour éviter de signaler les mêmes problèmes deux fois.
**How to apply:** Vérifier le statut de ces points avant chaque nouvel audit. Mettre à jour ce fichier si l'auteur confirme une résolution.
