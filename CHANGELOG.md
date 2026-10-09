# Changelog

## v1.1.0 — 2026-10-09

### Contenu
- Moyen mnémotechnique français corrigé : « Après Plusieurs Semaines, Tout Respire La Paix » (7 → 1).
- Couche 5 ajoutée à l'animation d'encapsulation (aller et retour) ; notes des couches 6 et 5 séparées.
- Nuance sur TLS : classé en couche 6 pour l'exercice, en réalité entre TCP et l'application.
- Couche 5 : « sockets de session » retiré, « SMB (négociation de session) » ajouté.
- Quiz, question 6 : mention de la variante à 5 couches du modèle TCP/IP.
- Références à un lab personnel remplacées par des formulations génériques ; bandeau « TAI / TSSR ».

### Accessibilité
- Couches OSI utilisables au clavier (boutons, `aria-pressed`, focus visible).
- Zones `aria-live` sur le détail des couches, la note d'animation et l'explication du quiz.

### Technique
- Tous les timers de l'animation sont annulés au Reset ; boutons verrouillés pendant l'animation.
- CSS mort supprimé, styles inline du tableau déplacés dans des classes.
- Mobile : la ligne « Couche 2 » n'est plus tronquée à 360 px.
- `<head>` : description, Open Graph, `theme-color`, favicon SVG inline, CSP ; message `<noscript>`.

### Documentation
- Mentions légales (LCEN) et licences dans le pied de page.
- `LICENSE` (MIT), `LICENSE-CONTENT.md` (CC BY-SA 4.0), `README.md`, `.gitignore`.

## v1.0.0

- Première version : pile OSI interactive, animation d'encapsulation, correspondance OSI / TCP-IP, quiz.
