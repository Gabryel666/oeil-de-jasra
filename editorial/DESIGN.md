# L’Œil de Jasra — Design System V4

## Intention

Un magazine numérique premium, sombre, élégant, éditorial, adulte et immersif, sans tomber dans le spectaculaire gratuit.

Le site doit rester excellent sur GitHub Pages : **statique, rapide, robuste, mobile-first**.

## Principes

- identité sombre et chaleureuse ;
- contraste fort mais non agressif ;
- typographie éditoriale expressive pour les titres ;
- interface sobre pour la navigation et les métadonnées ;
- grandes images, vrais rythmes de page, respirations généreuses ;
- hiérarchie claire entre grands articles, formats courts, données et coulisses ;
- cohérence stricte entre les numéros.

## Palette de base

La V4 peut faire évoluer légèrement la palette historique, mais conserve :

- fond nuit profond ;
- cartes légèrement plus claires ;
- or chaud comme accent principal ;
- accents secondaires contrôlés pour distinguer certaines rubriques ;
- texte principal ivoire/gris très clair ;
- texte secondaire plus doux.

## Typographie

- titres éditoriaux : sérif de caractère, lisible et premium ;
- navigation, labels, métadonnées : sans-serif nette et compacte ;
- largeur de ligne contrôlée pour les longs articles ;
- articles majeurs en colonne unique sur mobile ;
- colonnes desktop possibles uniquement lorsqu’elles améliorent réellement la lecture.

## Couverture

Chaque numéro doit avoir :

- une grande image hero ;
- numéro et période ;
- accroche éditoriale ;
- statistiques de veille discrètes ;
- sommaire cliquable ;
- transition visuelle nette vers le contenu.

## Articles majeurs

- grande image ou illustration ;
- légende/crédit ;
- titre fort ;
- chapô éventuel ;
- paragraphes confortables ;
- pullquotes sobres ;
- encarts de contexte ou chronologie lorsqu’utiles ;
- sources regroupées proprement en fin d’article.

## Formats courts

Buzz, critiques courtes, podcasts, crowdfunding et agenda doivent utiliser des cartes plus compactes, mais jamais donner une impression de dashboard SaaS. Le rendu reste éditorial.

## Interactions autorisées

Compatibles GitHub Pages et sans backend :

- liens d’ancrage ;
- sommaire sticky léger ;
- transitions CSS ;
- hover/focus sobres ;
- accordéons natifs (`details/summary`) si utiles ;
- lecture progressive ou reveal léger au scroll uniquement si le contenu reste totalement accessible sans JavaScript ;
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
- lazy-loading hors hero ;
- pas de JavaScript bloquant ;
- CSS mutualisé pour les nouveaux numéros ;
- préserver un rendu correct si une image distante disparaît ;
- éviter de dépendre d’URLs d’images temporaires ou hotlink-protected pour les visuels critiques.

## Responsive

Le mobile est un rendu de première classe, pas un fallback :

- pas de colonnes multiples étroites ;
- titres fluides ;
- cartes en pile ;
- marges adaptées ;
- images pleine largeur ;
- navigation utilisable au pouce ;
- pas de texte justifié si cela dégrade la lecture sur petit écran.

## Illustration

Le visuel doit servir l’article, pas simplement remplir une case.

- couverture : forte, mémorable ;
- dossier/À la Une : grande image ;
- critiques : visuels officiels privilégiés ;
- articles sans visuel satisfaisant : illustration générée cohérente avec la charte ;
- formats courts : vignette seulement si elle améliore le rythme visuel.

## Règle finale

Si un effet visuel est impressionnant mais fragile, lent ou dépendant d’une infrastructure non disponible sur GitHub Pages, **on choisit la version plus simple et mieux exécutée**.
