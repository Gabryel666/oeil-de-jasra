# L’Œil de Jasra — Charte éditoriale et visuelle V4

## Mission

L’Œil de Jasra est un magazine **hebdomadaire** d’actualité JDR, publié chaque vendredi matin sur GitHub Pages. Il doit être plus riche, plus approfondi et plus ambitieux que les numéros produits sous Hermes, tout en conservant la voix éditoriale de Jasra.

## Densité éditoriale

- Viser **8 000 à 12 000 mots** par numéro hebdomadaire lorsque l’actualité le permet.
- Ne jamais remplir artificiellement : la densité vient de la profondeur, du contexte et de la diversité des sujets.
- Chaque sujet majeur doit être un vrai article : accroche, contexte, faits, analyse, fermeture.
- Les formats courts doivent rester développés et sourcés, jamais réduits à une liste de titres.
- Toujours privilégier la matière utile : contexte historique, implications, réactions pertinentes, comparaison avec les développements précédents.

## Structure éditoriale de référence

La structure peut s’adapter à l’actualité, mais doit généralement couvrir :

1. Édito
2. À la Une
3. Grand Retour / grand sujet secondaire
4. Dossier ou enquête
5. Les Buzz
6. Nouvelles du front
7. Crowdfunding Watch international
8. Critiques
9. Podcasts / chaînes JDR
10. Coin des Geeks
11. Agenda
12. Crowdfunding francophone
13. En Coulisses — toujours en dernier

## Sources et vérification

- Chaque affirmation factuelle importante doit être reliée à une source identifiable.
- Croiser les faits sensibles, chiffres, dates, montants et annonces majeures.
- Distinguer clairement source primaire, presse, communauté et commentaire éditorial.
- Un sujet déjà traité ne revient que s’il existe un **nouvel état éditorial** : rumeur→confirmation, annonce→sortie, nominations→résultats, affaire→nouveau chapitre, etc.

## Sources évolutives

Le registre `editorial/sources.json` est vivant.

À chaque numéro :

- auditer les sources connues ;
- rechercher volontairement de nouvelles sources potentielles ;
- combler les catégories sous-couvertes ;
- tester les nouvelles sources ;
- classer chaque source comme `active`, `candidate`, `degraded` ou `rejected` ;
- ne jamais supprimer silencieusement une source ni perdre l’historique d’un rejet.

Une excellente source sans RSS peut rester active avec un suivi `web`.

## Illustration

Le magazine doit être richement illustré.

Priorité :

1. visuel officiel de l’éditeur ou de la source ;
2. visuel de campagne Kickstarter/Backerkit ou page produit ;
3. illustration encyclopédique/licite lorsque pertinente ;
4. **illustration générée** lorsqu’aucune image source satisfaisante n’existe ou lorsqu’un dossier mérite une direction artistique propre.

Exigences :

- une couverture visuellement forte ;
- au moins une illustration pour chaque article majeur ;
- vignettes lorsque cela améliore les formats courts ;
- crédit/source de l’image lorsque nécessaire ;
- vérifier que toute image distante utilisée pour les métadonnées OG répond correctement.

## Direction artistique

Le rendu doit être **premium, éditorial et adulte**, avec une identité sombre et élégante héritée des numéros précédents mais modernisée.

Principes :

- hiérarchie typographique forte ;
- grandes respirations ;
- contraste maîtrisé ;
- visuels éditoriaux généreux ;
- composants cohérents ;
- excellente lisibilité mobile ;
- design stable d’un numéro à l’autre.

### Contraintes GitHub Pages

Le site reste statique et compatible GitHub Pages :

- HTML5 sémantique ;
- CSS natif ;
- JavaScript léger uniquement lorsqu’il améliore réellement l’expérience ;
- aucun backend ;
- aucune dépendance serveur ;
- éviter les effets lourds, WebGL, animations coûteuses ou frameworks inutiles ;
- privilégier progressive enhancement, performances, accessibilité et résilience.

Les effets autorisés doivent rester sobres : transitions CSS, micro-interactions, sommaire sticky léger, ancres, révélation discrète au scroll si elle fonctionne sans dépendance lourde.

## Voix de Jasra

Jasra est la rédactrice en chef. Le ton doit être cultivé, vivant, personnel, parfois mordant, jamais plat ni publicitaire.

Les faits doivent rester rigoureux ; les jugements éditoriaux peuvent être assumés lorsqu’ils sont clairement présentés comme tels.

`En Coulisses` doit terminer le numéro avec un vrai regard de Jasra sur la semaine, la veille, les choix et les coulisses techniques.
