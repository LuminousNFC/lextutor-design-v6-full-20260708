# Design QA — V6 de référence

## Scope

- Homepage H-A consolidée : desktop 1440 px et mobile 390 px.
- Plateforme P-A consolidée : desktop 1440 px.
- Source visuelle : direction H-A / P-A validée.
- Contraintes : V6 comme base unique, contenu canonique inchangé, aucun nouveau concept.

## Reference and implementation

- Référence H-A / P-A : `https://luminousnfc.github.io/lextutor-design-v6-full-20260708/registre-preuve-20260710/`
- Implémentation locale : `dist/fr/index.html` et `dist/fr/plateforme.html`
- Planche comparative : `qa-reference/compare.html`

## Comparison history

1. Homepage desktop : hiérarchie et contenu conformes ; registre ramené de cinq à trois références visibles, deux références conservées dans un volet natif.
2. Homepage mobile : réduction nette de la longueur initiale ; ordre, CTA, références et statut conservés ; aucun débordement.
3. Plateforme introduction : proposition P-A reprise dans l’architecture V6 ; texte canonique complet conservé.
4. Plateforme graphe : relations nommées, direction unique, références réelles et nature illustrative des relations rendues lisibles sans animation.

## Severity review

### P0

- Aucun défaut bloquant observé.

### P1

- Aucun écart majeur de hiérarchie, de contenu, d’accessibilité ou de responsive observé.

### P2

- La typographie et les espacements restent ceux de la V6 afin de ne pas introduire une nouvelle direction.
- Le graphe final conserve le texte canonique additionnel de la V6 ; cet écart par rapport à la planche P-A est intentionnel et respecte la source de vérité éditoriale.

## Accessibility checks

- Un `h1` par page.
- Registre avec rôles de tableau, ligne et cellule.
- Volets avec `details` / `summary` natifs.
- Navigation, CTA, vidéo, FAQ et liens utilisables au clavier.
- Focus visible et contraste de texte conservés.
- Aucun contenu indispensable dépendant d’une animation, d’un hover ou d’une couleur seule.
- Test des petites cibles interactives : 0 anomalie détectée sur les surfaces contrôlées.

## Performance checks

- Vidéo `preload="none"`, sans autoplay.
- Aucune ressource MP4 ou WebM chargée avant action utilisateur.
- Animations actives après introduction : 0 sur les pages consolidées.
- Flou et grain décoratif désactivés.
- Console : 0 erreur.
- Images cassées : 0.

## Automated checks

- `python3 -m py_compile build6.py` : réussi.
- `python3 build6.py` : 50 fichiers générés.
- `node qa-v6full-local.mjs` : 88 pages/vues valides, 0 anomalie.
- Largeurs contrôlées : 375 px et 1440 px.

## Final result

passed
