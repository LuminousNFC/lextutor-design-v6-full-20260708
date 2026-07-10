# Gate visuel — extension de la grammaire P-A

Statut : rendu local, non publié.

## Structure avant / après

| Page | Avant | Après local | Artefact propre |
|---|---|---|---|
| Homepage | H-A consolidée, registre initial et vidéo | Inchangée ; compatible avec les mêmes marges, statuts et tokens | Registre de preuve initial |
| Plateforme | P-A consolidée | Référence de grammaire, inchangée | Cinq couches + graphe d’autorité |
| Solutions | Flux éditorial intégral, usages et preuves au même niveau | Introduction, index métier, quatre registres ; douleur visible, usage et preuve repliables | Registres métier |
| Bench | Sections éditoriales sans points méthodologiques ni tableau visible | Principes visibles, axes méthodologiques repliables, tableau FR/DE/IT restauré | Registre de mesure |
| Sécurité | Long flux de claims, détails et statuts | Cartographie des cinq couches visible ; détails contractuels et gated au second niveau ; FAQ native | Registre des flux |
| À propos | Suite de paragraphes | Mission, doctrine, signature et engagement séparés ; quatre principes restaurés sous forme de registre | Registre des engagements |
| Méthodologie | Suite générique de sections | Séquence numérotée et reliée comme un dossier ; liste des trois mesures restaurée | Dossier en constitution |
| Tarifs | Deux variantes affichées intégralement à la suite | Offre principale structurée en registre ; FAQ repliable ; variante secondaire conservée en annexe repliable | Registre d’offre |
| Contact | Trois blocs éditoriaux | Introduction puis trois étapes courtes et actionnables | Ouverture du dossier |
| Mentions légales | Flux générique | Introduction légale, index, cinq articles numérotés | Registre légal sobre |
| Protection des données | Flux générique | Introduction, index et déclaration structurée par objet | Registre de traitement |

## Contenus déplacés ou repliés

- Solutions : « Usage type » et « La preuve LexTutor » sont repliés pour chaque métier. Les douleurs, bandeaux et signatures restent au premier niveau.
- Bench : les trois axes détaillés de méthodologie sont repliés sous leurs titres canoniques. Les principes de scoring et le tableau de résultats restent visibles.
- Sécurité : les précisions contractuelles, mécanismes, politiques d’accès, certifications et transferts non validés sont regroupés sous « Détails partagés en rendez-vous privé ». La localisation par couche, les claims principaux et l’art. 321 CP restent visibles.
- Sécurité : les cinq questions fréquentes sont converties en accordéons natifs.
- Tarifs : les questions tarifaires sont repliées ; la variante B entière est conservée comme annexe repliable. Aucun prix ou engagement n’est inventé.
- Les placeholders B1/B3/B4/B5/STAT restent représentés par le statut canonique « Sur rendez-vous » ; ils ne sont ni supprimés ni remplacés par des faits.
- À propos : aucun paragraphe n’est replié ; les quatre principes précédemment omis par le parseur sont restaurés au premier niveau.
- Méthodologie : aucun contenu n’est replié ; les trois critères précédemment omis sont restaurés dans la séquence.

## QA

- Génération : 50 fichiers, 4 langues × 11 pages + racine.
- Responsive automatisé : 88 vues contrôlées à 375 px et 1440 px ; 0 débordement.
- Gate visuel : 1440 px desktop et 390 px mobile pour Solutions, Bench, Sécurité et À propos.
- Sémantique : un `h1` par page ; tableaux avec en-têtes ; accordéons natifs `details/summary`.
- Clavier : accordéons ouverts avec Entrée ; menu mobile ouvert avec Entrée ; focus visible de 2 px.
- Cibles interactives : 0 cible visible sous 24 px sur les huit vues du gate.
- Reduced motion : 0 animation active sur les huit vues sous `prefers-reduced-motion: reduce`.
- Console : 0 erreur sur les huit vues.
- Publication : non effectuée ; gate visuel en attente de validation.
