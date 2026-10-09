# OSI & TCP/IP — les couches réseau, décortiquées

Une fiche de révision interactive pour comprendre les modèles OSI et TCP/IP, en une seule page HTML.

[![Code : MIT](https://img.shields.io/badge/code-MIT-blue)](LICENSE)
[![Contenu : CC BY-SA 4.0](https://img.shields.io/badge/contenu-CC%20BY--SA%204.0-lightgrey)](LICENSE-CONTENT.md)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-en%20ligne-2ea44f)](https://anotherj4ck.github.io/osi-tcpip/)
![HTML/CSS/JS — zéro dépendance](https://img.shields.io/badge/HTML%2FCSS%2FJS-z%C3%A9ro%20d%C3%A9pendance-orange)

**Démo en ligne : https://anotherj4ck.github.io/osi-tcpip/**

![Capture d'écran de la fiche OSI / TCP-IP](docs/capture.png)

## Fonctionnalités

- **Pile OSI cliquable** : rôle, unité de données (PDU) et protocoles concrets pour chacune des 7 couches, au clic ou au clavier.
- **Animation d'encapsulation** : les en-têtes s'ajoutent couche par couche à l'envoi, puis se retirent à la réception.
- **Correspondance OSI / TCP-IP** : tableau qui montre comment les 7 couches OSI se regroupent dans les 4 couches TCP/IP.
- **Quiz de 8 questions** avec une explication après chaque réponse et un score final.

## Pourquoi ce projet

J'ai construit cette fiche pendant ma formation TAI pour réviser les modèles réseau, avec en ligne de mire le titre TSSR. Plutôt qu'un résumé figé, je voulais un support qu'on manipule : cliquer une couche, voir un paquet s'encapsuler, se tester tout de suite.

## Choix techniques

- **Fichier unique** : tout tient dans `index.html` (HTML, CSS et JS inline), sans build ni framework. La page s'ouvre aussi bien en local qu'en ligne.
- **Aucune dépendance ni requête externe** : pas de CDN, pas de police web, pas de traceur. Le visiteur ne contacte aucun tiers, donc il n'y a rien à déclarer côté RGPD.
- **Content Security Policy** : une balise `<meta http-equiv="Content-Security-Policy">` interdit tout chargement extérieur (`default-src 'none'`). Le JS n'utilise `innerHTML` qu'avec des données statiques écrites dans le fichier.
- **Accessibilité clavier** : les couches OSI sont de vrais boutons (`aria-pressed`) avec un focus visible ; les zones qui changent sont annoncées aux lecteurs d'écran (`aria-live`).
- **`prefers-reduced-motion`** : si le système demande moins d'animations, les transitions sont coupées.

## Lancer en local

Ouvrir `index.html` dans un navigateur suffit. Pour servir la page comme sur GitHub Pages :

```sh
# Linux
python3 -m http.server 8000
```

```powershell
# Windows
py -m http.server 8000
```

Puis aller sur http://localhost:8000.

## Licences

- Code (HTML, CSS, JS) : [MIT](LICENSE).
- Contenu pédagogique (textes, quiz, explications) : [CC BY-SA 4.0](LICENSE-CONTENT.md).

## Mentions légales

Les mentions légales (éditeur, hébergeur, données personnelles) sont dans le pied de page du site, rubrique « Mentions légales & licence ».
