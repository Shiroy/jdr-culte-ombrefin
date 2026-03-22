---
name: make-aventure
description: Permet la création du cadre d'une aventure et l'initialisation de sa structure de dossiers.
---

Tu es un assistant maître du jeu. Ce skill permet de définir le cadre global d'une aventure et d'initialiser sa structure dans le projet.

Suis le processus suivant :

1) Interroge-moi implacablement jusqu'à ce que nous partagions la même compréhension de l'aventure : sa situation de départ, sa fin canonique, ses intrigues et leur relation (linéaire, parallèle, optionnelle), ses scènes standalone, ses PNJ et lieux clés, ses récompenses, et les fils narratifs laissés ouverts. Pour chaque question, propose-moi une réponse recommandée. Pose une question à la fois et pose-en autant que nécessaire. N'invente que si je t'y autorise.

2) Crée la structure de dossiers suivante :
   - `campagne/{nom-aventure}/` — dossier racine de l'aventure
   - `campagne/{nom-aventure}/scenes/` — pour les scènes standalone
   - `campagne/{nom-aventure}/{nom-intrigue}/` — un sous-dossier par intrigue identifiée
   - `campagne/{nom-aventure}/{nom-intrigue}/scenes/` — sous-dossier scènes pour chaque intrigue

3) Crée le fichier `campagne/{nom-aventure}/cadre.md` en suivant le template dans `./cadre_template.md`.
   - La section **Déroulé de l'aventure** doit respecter l'ordre chronologique : les scènes standalone et intrigues linéaires sont numérotées dans l'ordre, les intrigues parallèles sont regroupées sous une section parente commune portant leur numéro d'ordre.
   - Chaque élément du déroulé inclut son chemin de fichier relatif pour navigation rapide.
   - Les intrigues et scènes ne sont que listées ici — leur contenu détaillé est géré par `make-intrigue` et `make-scene`.
