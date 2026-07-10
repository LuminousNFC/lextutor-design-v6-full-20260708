# V6 de référence — consolidation H-A / P-A

Date : 10 juillet 2026

Base unique : V6 fonctionnelle

Périmètre : Homepage et Plateforme, quatre langues

## Résultat

La V6 devient la version fonctionnelle de référence. L’architecture, les contenus éditoriaux, les références juridiques, les liens et les parcours existants sont conservés. Aucune variante, aucun claim et aucun parcours n’ont été ajoutés.

## Homepage — desktop et mobile

- Hiérarchie du hero allégée sans modifier son contenu : eyebrow, proposition, explication, deux actions, puis registre.
- Registre initial limité aux trois références nécessaires à la compréhension immédiate : CO art. 367, CO art. 368 et ATF 136 III 273.
- CO art. 371 al. 2 et ATF 130 III 362 restent disponibles dans un volet natif « 2 sources complémentaires ».
- Statut de démonstration rendu unique et constant : `CORPUS PUBLIC · DÉMONSTRATION STATIQUE`.
- Suppression du badge décoratif « Hébergé en Suisse » et de l’instruction de survol.
- Suppression du relief décoratif du registre ; maintien des codes couleur uniquement lorsqu’ils expriment la nature d’une source.
- Vidéo conservée, mais sans lecture automatique ni préchargement média avant action explicite.
- Mise en page mobile consolidée sans débordement horizontal.

## Plateforme — desktop

- Reprise verbatim du contenu canonique `contenu/v1/plateforme.{lang}.md`.
- Conservation des cinq couches et de leur ordre.
- Navigation latérale de lecture ajoutée à partir des titres existants, sans créer de nouveau parcours.
- Artefacts de preuve associés aux cinq couches à partir des références et libellés déjà présents.
- Graphe d’autorité placé uniquement dans la section qui décrit les relations entre sources.
- Sens de lecture rendu explicite : Question → lois fédérales → jurisprudence → analyse.
- Références signalées comme réelles et relations comme illustratives.
- FAQ rendue avec des éléments natifs repliables.
- Statuts de démonstration harmonisés avec la homepage.

## Accessibilité et performance

- Un seul `h1` par page ; structure sémantique conservée.
- Registre exposé comme tableau sémantique, avec en-têtes, lignes et cellules.
- Contrôles natifs pour les sources complémentaires et la FAQ.
- Cibles interactives secondaires portées à 24 px minimum ; contrôles principaux à 44 px ou plus.
- Focus clavier visible conservé.
- Animations de révélation et grain décoratif désactivés sur les deux pages consolidées.
- `prefers-reduced-motion` respecté.
- Suppression du flou de navigation sur ces pages.
- Aucune requête vidéo avant interaction ; images sans erreur de chargement.

## Éléments volontairement inchangés

- Architecture globale et navigation V6.
- Contenus, claims, références, liens officiels et appels à l’action.
- Routes et alternates linguistiques.
- Les neuf autres pages de la V6.
- Aucun fichier de production externe, aucun nouveau dépôt et aucune nouvelle direction visuelle.

## Vérifications

- Génération : 50 fichiers, soit 4 langues × 11 pages + racine.
- QA automatisée : 88 vues vérifiées à 375 px et 1440 px, aucune anomalie.
- Navigation mobile et changement de langue vérifiés.
- Homepage desktop et mobile : aucun débordement horizontal.
- Plateforme desktop : aucun débordement horizontal.
- Compréhension statique du registre et du graphe vérifiée sans animation.
- Console navigateur : aucune erreur.
