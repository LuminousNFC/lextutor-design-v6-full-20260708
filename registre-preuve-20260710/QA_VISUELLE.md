# QA visuelle — H-A et P-A

Date : 10 juillet 2026  
Viewports : 1440 × 1000 et 390 × 844.  
Statut : maquettes isolées, non intégrées.

## Résultats synthétiques

| Vue | Hauteur | Écrans | Overflow horizontal | Animations | Images cassées | Cibles < 24 px | Scripts |
|---|---:|---:|---:|---:|---:|---:|---:|
| H-A desktop | 3 544 px | 3,54 | 0 | 0 | 0 | 0 | 0 |
| H-A mobile | 4 730 px | 5,60 | 0 | 0 | 0 | 0 | 0 |
| P-A desktop | 6 056 px | 6,06 | 0 | 0 | 0 | 0 | 0 |

## Compréhension statique

- H-A desktop : la promesse, les deux CTA et le registre complet sont visibles dans le premier chapitre. Le registre peut être compris sans survol ni animation.
- H-A mobile : la promesse et les actions précèdent le registre ; chaque source est affichée comme une ligne autonome avec statut et lien officiel.
- P-A desktop : les cinq couches restent numérotées et nommées dans le contenu. L’index latéral est secondaire ; il n’est pas nécessaire pour comprendre la page.
- Le graphe est nommé, légendé et marqué comme illustratif. Les références proviennent de la maquette actuelle.

## Longueur

- H-A desktop est ramenée à 3,54 écrans ; aucune section intermédiaire décorative.
- H-A mobile reste plus longue en raison du registre linéarisé, mais n’impose aucun carrousel ni défilement horizontal.
- P-A desktop conserve les cinq textes canoniques. Les questions techniques utilisent des éléments `details` natifs fermés par défaut, ce qui évite d’ajouter plusieurs écrans sans supprimer le contenu.

## Accessibilité

- Un seul `h1` par page.
- Aucun débordement horizontal aux viewports contrôlés.
- Aucun élément interactif inférieur à 24 × 24 px lors du contrôle automatisé.
- Les liens officiels restent nommés ; l’état n’est pas communiqué uniquement par la couleur.
- Les lignes du registre mobile disposent d’un libellé accessible complet.
- Contrastes mesurés : encre/papier 17,76:1 ; gris/papier 4,59:1 ; vert texte/blanc 5,02:1 ; violet/blanc 7,10:1 ; orange texte/papier 6,24:1 ; blanc/encre 18,22:1.
- Le carré de validation conserve la couleur V7 `#168A45`. Les petits textes verts utilisent `#15803D` pour le contraste.
- `prefers-reduced-motion` est présent, même si ces maquettes statiques ne lancent aucune animation.
- Limite : un contrôle clavier et lecteur d’écran complet restera nécessaire avant toute intégration.

## Performance

- Aucun JavaScript et aucun canvas.
- Aucune vidéo, police distante ou bibliothèque externe.
- CSS partagé : environ 14 Ko transférés à froid.
- Logo V7 : moins de 1 Ko transféré.
- Le graphe est statique ; une version future devra rester SVG léger avec fallback liste.

## Verrou d’intégration

Ces fichiers servent uniquement à la validation visuelle. Ils ne doivent être copiés, fusionnés, publiés ou intégrés au site qu’après validation explicite des captures par Daniel.
