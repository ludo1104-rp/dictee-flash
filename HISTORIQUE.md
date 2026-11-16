# Historique — Dictée flash

## Retiré de CLAUDE.md le 13/11/2026

### Journal des versions (ancien « État »)
- 1.6 (publiée le 04/11/2026) : bouton QR code (icône ronde, en haut à droite
  à côté des Réglages, accueil seulement, `#qrBtn`)
  (`openQR()`, fenêtre `#qrModal`). Grand QR noir sur blanc pour le TVI, points et coins arrondis,
  créé dans la page (hors ligne). Adresse = la page en ligne, ou `APP.lien`
  si ouverte depuis le Mac. Code commun : skill `assets/qr-partage.js`.
  Testé : se lit bien (lecteur de Chromium), iPad et Mac OK.
- 1.5 publiée le 24/10/2026 : pendant la dictée, bouton « Vérifier »
  (phase `verif` : le mot revient en vert, sans minuteur, puis « Mot suivant »)
  et bouton « Retour » (`reculer()` : en lecture → mot précédent ; en écriture
  ou vérification → revoir le mot). Flèche gauche du clavier = Retour.
- 1.4 publiée le 23/10/2026 : style Simple = charte de rprof1.com
  (police Figtree incluse, noir et gris, pastels gardés pour les réponses).
  Pied de page : « Ludo (@rprof_1) » au lieu du nom complet.
  Étiquette « Nouveau » sur le bouton Simple (3 ouvertures ou un toucher).
  Réponses en vrai pastel, animation du point à l’ouverture (`ouverture()`).
  Retour en arrière : `git reset --hard avant-style-site`.
- Version 1.3 publiée le 23/10/2026 : https://ludo1104-rp.github.io/dictee-flash/
  (dépôt public ludo1104-rp/dictee-flash, branche main, GitHub Pages).
- 1.3 : accueil court (titre, consignes, Commencer), puis 3 étapes sans
  défilement : 1 Les mots, 2 Le rythme, 3 Affichage et son → « Commencer la
  dictée ». Boutons Retour/Suivant fixés en bas (`renderEtape(n)`, `ETAPES`).
  Étape 1 bloquée tant que le cadre est vide. Bouton Plein écran retiré (choix de Ludo).
- Copiée depuis `~/Desktop/Claude Code/dictee-flash-v1.1.html` (les anciennes
  versions restent sur le bureau).
- 1.2 : bouton « Mots au hasard » dans le cadre des mots. Il tire
  10 mots (`NB_HASARD`) dans `MOTS_BASE` (400 mots, 8-9 ans). Si le cadre
  contient déjà des mots, il faut toucher deux fois pour remplacer.
- La liste `MOTS_BASE` (400 mots) a été écrite par DeepSeek et relue par
  Claude (orthographe, doublons). DeepSeek n'a pas pu consulter de liste
  officielle FWB : **à relire par Ludo**.
- Licence CC BY-NC-SA 4.0 : mention en bas de l'accueil + fichier `LICENSE`.
- 24/10/2026 : logo « Ludo. » tout en haut à gauche de l'accueil (déplacé et publié le 24/10, non cliquable) + lien rprof1.com dans les mentions (publié le 24/10/2026).

### Notes datées (ancien « Prochaine étape »)
- 25/10/2026 aussi : gris `--muted` foncé (#5F6A76), mentions en 14 px.
25/10/2026 (publié) : double appui sur « J'écris » ignoré
(400 ms, sinon l'élève sautait l'écriture du mot) ; ligne « Monet » retirée
de LICENSE. Testé.
- 23/10/2026 : signature « Ludo. » (point en gras) dans les mentions, publiée.
- 28/10/2026 (publié) : accueil allégé comme la Foire de Liège. Style et taille du texte rangés dans « Réglages » (bouton à côté du haut-parleur, `openRegl()`).
