# Design QA — extension P-A à toutes les pages

## Evidence

- Source visuelle : `gate-visual/reference-plateforme-desktop.png`
- Implémentations desktop : `gate-visual/{solutions,bench,securite,a-propos}-desktop.png`
- Implémentations mobile : `gate-visual/{solutions,bench,securite,a-propos}-mobile.png`
- Planche combinée : `gate-visual/index.html`
- Viewports : 1440 × 1000 et 390 × 844 ; pages complètes capturées.
- État : accordéons fermés pour évaluer le premier niveau de lecture.

## Required fidelity surfaces

- Typography: mêmes familles, poids, échelle, césure et hiérarchie que P-A ; un seul `h1` par page.
- Spacing and layout: introduction ample, index, grille latérale et rythme de sections communs ; densité réduite par niveaux de lecture.
- Colors and tokens: palette papier, encre, orange d’analyse, vert loi et violet jurisprudence inchangée ; aucun nouveau code décoratif.
- Image quality: aucune image ou illustration ajoutée ; aucune substitution d’asset. Les pages reposent sur les artefacts documentaires canoniques.
- Copy and content: textes issus des fichiers `contenu/v1`; listes, FAQ, axes du Bench et tableau de mesure restaurés ; placeholders conservés comme statuts.

## Comparison history

1. P1 — Sécurité : les cellules du registre de flux se repliaient dans une colonne trop étroite. Fix : contenu de chaque ligne enveloppé sémantiquement et grille du flux dédiée. Post-fix : lecture horizontale desktop et empilement mobile sans débordement.
2. P1 — Complétude : les listes imbriquées, les axes numérotés du Bench, les FAQ et le tableau de mesure n’étaient pas récupérés par le parseur historique. Fix : parse des bullets, clés numérotées, paires Q/R, tables et liens. Post-fix : tous ces éléments sont visibles ou repliables.
3. P2 — Hiérarchie : les pages partageaient initialement un rendu trop uniforme. Fix : registres métier, mesure, flux et engagements distincts ; niveaux secondaires repliés.
4. P2 — Accessibilité : quelques liens textuels mesuraient 19–22 px de haut. Fix : hauteur interactive minimale de 24 px. Post-fix : 0 petite cible détectée.
5. P1 — Cohérence de grille : les pages P-A utilisaient un conteneur de 1200 px contre 1120 px sur la homepage. Fix : largeur commune de 1120 px. Post-fix à 1900 px : conteneur `x=390`, logo et contenu `x=418` sur toutes les routes contrôlées.
6. P1 — Index incomplets : les intitulés étaient tronqués par `text-overflow: ellipsis`. Fix : suppression de l’ellipsis et retour à la ligne naturel. Post-fix : 0 libellé d’index dont `scrollWidth` dépasse `clientWidth`.
7. P1 — Registre des flux : les badges de statut occupaient une cellule de grille autonome et se repliaient verticalement. Fix : cellules sémantiques distinctes `flow-title` et `flow-detail`, statut intégré au détail. Post-fix : badges à largeur normale, aucune colonne parasite et aucun débordement.

## Focused comparisons

- Solutions : douleur visible, usage et preuve dans deux accordéons par métier.
- Bench : trois principes et registre de mesure visibles ; axes détaillés repliés.
- Sécurité : cinq couches visibles avec statut ; détails contractuels et FAQ repliables.
- À propos : doctrine mise en regard d’un registre de quatre engagements, sans accordéon.

## Interaction and accessibility checks

- Accordéons Solutions, Bench et Sécurité ouverts au clavier avec Entrée.
- Menu mobile ouvert au clavier sur les quatre pages.
- Focus visible : 2 px.
- Reduced motion : 0 animation active.
- Débordement horizontal : 0 à 390 px et 1440 px.
- Intitulés d’index tronqués : 0 sur les 22 vues finales.
- Alignement desktop : grille commune vérifiée sur homepage, Plateforme, Solutions, Bench, Sécurité et À propos.
- Console browser : 0 erreur.

## Findings

- Aucun P0, P1 ou P2 restant sur les huit vues du gate.
- P3 : les libellés d’index sont volontairement tronqués sur desktop et réduits à leur numéro sur mobile ; le titre complet reste visible dans chaque section.

## Publication gate

La publication est volontairement suspendue jusqu’à validation visuelle explicite.

## final result

passed
