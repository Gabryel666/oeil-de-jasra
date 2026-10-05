# L’Œil de Jasra — Design System V4.1

## Intention

Un magazine numérique premium, sombre, élégant, éditorial, adulte et immersif, avec une vraie ambition de composition. Le site doit rester excellent sur GitHub Pages : **statique, rapide, robuste, mobile-first**.

## Principe directeur

Ne jamais retomber dans une simple succession de blocs identiques. Chaque numéro doit avoir du rythme : grands moments, respirations, compositions asymétriques, cartes courtes, rubriques visuellement différenciées.

Le design peut être audacieux tant qu’il reste lisible, stable et compatible GitHub Pages.

## Principes

- identité sombre et chaleureuse ;
- contraste fort mais non agressif ;
- typographie éditoriale expressive pour les titres ;
- interface sobre pour la navigation et les métadonnées ;
- masthead et couverture visuellement forts ;
- grandes images, vrais rythmes de page, respirations généreuses ;
- compositions asymétriques sur desktop lorsque cela sert la lecture ;
- hiérarchie claire entre grands articles, formats courts, données et coulisses ;
- cohérence stricte entre les numéros sans imposer une grille rigide.

## Palette de base

- fond nuit profond ;
- cartes légèrement plus claires ;
- or chaud comme accent principal ;
- accents secondaires contrôlés ;
- texte principal ivoire/gris très clair ;
- texte secondaire plus doux.

## Typographie

- titres éditoriaux : sérif de caractère, lisible et premium ;
- navigation, labels, métadonnées : sans-serif nette et compacte ;
- très grands titres autorisés pour le masthead et les articles majeurs ;
- largeur de ligne contrôlée pour les longs articles ;
- alignements précis et cohérents ;
- éviter tout effet de titre flottant ou mal raccordé aux visuels ;
- mobile : colonne unique confortable, titres fluides, aucun texte tassé.

## Couverture

Chaque numéro doit avoir :

- un masthead fort ;
- une grande image hero ou une illustration locale ;
- numéro et période ;
- accroche éditoriale ;
- métadonnées de numéro discrètes ;
- sommaire cliquable ;
- transition visuelle nette vers le contenu.

## Articles majeurs

- grande image ou illustration ;
- titre fort ;
- chapô éventuel ;
- paragraphes confortables ;
- pullquotes sobres ;
- encarts de contexte ;
- sources regroupées proprement en fin d’article ;
- compositions variées d’un grand article à l’autre.

## Formats courts

Buzz, critiques courtes, podcasts, crowdfunding, agenda et petites news doivent être **visuellement illustrés par défaut** lorsque cela apporte du relief.

Les cartes courtes :
- gardent un rendu éditorial, pas un dashboard SaaS ;
- utilisent une vignette ou une illustration locale ;
- conservent une vraie hiérarchie titre / texte / méta ;
- restent alignées en hauteur et espacées proprement dans une même grille.

## Illustration

Le visuel sert l’article, mais le magazine doit être richement illustré.

- couverture : forte, mémorable ;
- dossier / À la Une : grande image ;
- critiques : visuels officiels privilégiés ;
- petites news : vignette par défaut si possible ;
- articles sans visuel satisfaisant : illustration générée ou SVG éditorial cohérent ;
- préférer les assets locaux pour les visuels critiques afin d’éviter les hotlinks fragiles.

## Interactions autorisées

Compatibles GitHub Pages et sans backend :

- liens d’ancrage ;
- sommaire sticky léger ;
- transitions CSS ;
- hover/focus sobres ;
- accordéons natifs (`details/summary`) si utiles ;
- reveal léger au scroll uniquement si le contenu reste totalement accessible sans JavaScript ;
- bouton retour en haut léger.

## Interactions à éviter

- WebGL ;
- canvas animé lourd ;
- parallaxe agressive ;
- vidéo autoplay ;
- carrousels complexes ;
- frameworks JS lourds uniquement pour l’apparence ;
- dépendances nécessitant un serveur ;
- animations essentielles à la compréhension ;
- effets qui dégradent fortement mobile ou accessibilité.

## Performance

- images dimensionnées et compressées ;
- lazy-loading hors hero lorsque pertinent ;
- pas de JavaScript bloquant ;
- CSS séparé des gros fichiers HTML lorsqu’un numéro devient complexe ;
- assets locaux privilégiés pour la couverture et les visuels structurants ;
- préserver un rendu correct si une image distante disparaît.

## Responsive

Le mobile est un rendu de première classe, pas un fallback :

- pas de colonnes multiples étroites ;
- titres fluides ;
- cartes en pile ;
- marges adaptées ;
- images pleine largeur ;
- navigation utilisable au pouce ;
- pas de texte justifié si cela dégrade la lecture sur petit écran.

## Règle finale

Si un effet visuel est impressionnant mais fragile, lent ou dépendant d’une infrastructure non disponible sur GitHub Pages, **on choisit la version plus simple et mieux exécutée**. En revanche, la contrainte technique ne doit jamais devenir une excuse pour revenir à un design timide ou répétitif.
