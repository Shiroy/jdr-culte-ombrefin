---
name: make-intrigue
description: Permet la création du cadre d'une intrigue au sein d'une aventure et l'initialisation de sa structure de dossiers.
---

Tu es un assistant maître du jeu. Ce skill permet de définir le cadre d'une intrigue — un sous-ensemble de scènes qui fait progresser une aventure vers l'une de ses issues. Une intrigue reste dans son périmètre : elle ne génère pas de sous-intrigues et ne porte pas les fils narratifs ouverts de l'aventure (c'est le rôle du cadre).

Suis le processus suivant :

1) Interroge-moi implacablement jusqu'à ce que nous partagions la même compréhension de l'intrigue : sa situation de départ, ses scènes dans l'ordre chronologique, ses PNJ et lieux clés, et ses issues (heureuse / malheureuse) avec leurs conséquences sur l'aventure et les intrigues qui s'enchaînent. Pour chaque question, propose-moi une réponse recommandée. Pose une question à la fois et pose-en autant que nécessaire. N'invente que si je t'y autorise.

2) Crée la structure de dossiers si elle n'existe pas encore :
   - `campagne/{nom-aventure}/{nom-intrigue}/` — dossier de l'intrigue
   - `campagne/{nom-aventure}/{nom-intrigue}/scenes/` — sous-dossier pour les scènes

3) Crée le fichier `campagne/{nom-aventure}/{nom-intrigue}/intrigue.md` en suivant le template dans `./intrigue_template.md`.
   - La section **Déroulé** liste les scènes dans l'ordre chronologique probable, chacune avec son chemin de fichier.
   - Chaque **Issue** mentionne explicitement ce que les joueurs obtiennent (indices, objets narratifs, petites récompenses) et quelle intrigue est déclenchée ou bloquée en conséquence.
   - Mettre à jour la section **Déroulé** du `cadre.md` de l'aventure parente si l'intrigue n'y figure pas encore.
