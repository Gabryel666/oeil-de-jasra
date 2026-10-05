# L’Œil de Jasra — Workflow de production V4

## Cadence

Publication **hebdomadaire, chaque vendredi matin**.

La tâche planifiée ChatGPT doit lancer la production suffisamment tôt pour terminer recherche, rédaction, mise en page, publication et contrôle du site le vendredi matin.

## Source de vérité

Avant toute production, lire :

- `editorial/CHARTE.md`
- `editorial/WORKFLOW.md`
- `editorial/sources.json`
- `editorial/state.json`
- le hub `index.html`
- les numéros précédents

Ne jamais privilégier la mémoire conversationnelle lorsqu’une information contradictoire existe dans le dépôt.

## Pipeline

### 1. État et reprise

Lire `editorial/state.json`.

- déterminer le prochain numéro ;
- déterminer la période éditoriale depuis le dernier numéro publié ;
- si une production est déjà en cours, reprendre cette production au lieu d’en créer une seconde ;
- ne modifier `last_published_issue` qu’après vérification du site réellement publié.

### 2. Audit des sources

Pour toutes les sources actives :

- vérifier accessibilité et fraîcheur ;
- relever les sources silencieuses ou dégradées ;
- conserver l’historique des changements d’état.

### 3. Découverte de nouvelles sources

Étape obligatoire à chaque numéro.

- rechercher volontairement de nouvelles sources JDR FR et internationales ;
- cibler en priorité les catégories insuffisamment couvertes ;
- inclure blogs, presse, éditeurs, podcasts, YouTube, crowdfunding, forums, communautés, outils et releases ;
- RSS/Atom préféré quand disponible, mais une excellente source Web sans RSS peut être intégrée.

Évaluer chaque candidate : pertinence JDR, fraîcheur, fiabilité, fréquence, langue, originalité, signal/bruit, redondance avec les sources existantes.

Mettre à jour `editorial/sources.json`.

### 4. Collecte de la période

Analyser toute la période depuis la clôture du dernier numéro.

Ne pas se limiter aux flux RSS : compléter par une recherche Web large afin de détecter les annonces importantes absentes des sources enregistrées.

### 5. Normalisation et clustering

- normaliser titres, URL, source, date de publication et date de l’événement ;
- dédupliquer ;
- regrouper les articles relatifs au même événement ;
- identifier la source primaire lorsque possible.

### 6. Anti-doublon éditorial

Relire les précédents numéros avant sélection.

Un sujet déjà couvert ne revient que si l’histoire a réellement évolué :

- rumeur → officialisation ;
- leak → confirmation ;
- annonce → publication ;
- nominations → résultats ;
- affaire → nouveau chapitre.

### 7. Sélection et profondeur

Sélectionner selon : importance, nouveauté, intérêt JDR, potentiel éditorial, diversité FR/VO, diversité des systèmes et acteurs.

Objectif hebdomadaire : matière abondante et approfondie, sans remplissage.

### 8. Fact-check

Avant rédaction finale :

- vérifier noms propres ;
- dates ;
- durées ;
- chiffres ;
- montants ;
- citations ;
- statut réel des annonces ;
- liens sources.

Toute information incertaine doit être signalée ou écartée.

### 9. Rédaction

Respecter `CHARTE.md`.

Le numéro doit viser 8 000–12 000 mots lorsque la matière le permet et offrir davantage de contenu que les numéros Hermes.

### 10. Illustrations

Pour chaque article majeur :

- chercher d’abord une illustration officielle ou issue de la source ;
- si aucune illustration satisfaisante n’existe, prévoir une illustration originale générée ;
- vérifier dimensions, pertinence, crédit et disponibilité ;
- choisir une image principale forte pour l’OG et la couverture.

### 11. Production Web premium

Conserver GitHub Pages comme canal de publication.

Le rendu doit rester statique et robuste : HTML/CSS, JavaScript léger seulement.

Ne jamais sacrifier performance, mobile ou accessibilité pour un effet décoratif.

### 12. Branche de production

Pour chaque numéro, travailler sur une branche `jasra/numero-N`.

Ne pas pousser directement une production incomplète sur `main`.

Créer ou mettre à jour :

- le dossier `numero-N/` ;
- le hub `index.html` ;
- `editorial/sources.json` ;
- `editorial/state.json` ;
- `editorial/runs/numero-N.md`.

### 13. Contrôle qualité

Avant publication vérifier :

- suffisamment de matière ;
- structure complète et cohérente ;
- absence de doublons éditoriaux injustifiés ;
- liens sources présents ;
- faits sensibles vérifiés ;
- illustrations présentes et fonctionnelles ;
- page responsive ;
- métadonnées OG cohérentes ;
- pas de dépendance incompatible avec GitHub Pages.

### 14. Publication

Créer une PR de production vers `main`.

Si les permissions permettent le merge sans approbation supplémentaire et que tous les contrôles sont satisfaits, fusionner la PR. Sinon laisser la PR prête et signaler l’action requise.

### 15. Vérification live

Après merge :

- vérifier l’URL du nouveau numéro ;
- vérifier le hub ;
- vérifier l’image OG ;
- ne jamais annoncer une publication réussie avant que la page réelle soit accessible.

### 16. Journal et En Coulisses

Écrire `editorial/runs/numero-N.md` avec :

- période ;
- volume analysé ;
- sources actives ;
- nouvelles sources trouvées ;
- candidates ;
- sources dégradées/rejetées ;
- sujets retenus ;
- sujets importants écartés ;
- anomalies de production.

Cette matière alimente `En Coulisses`.
