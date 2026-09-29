# Télécom 3 — Carnet de révision R306

Site statique en français pour le BUT Réseaux & Télécommunications, semestre 3, 2026–2027.

## Contenu

- 8 fiches organisées selon les 3 thèmes des supports : propagation, transmissions optiques et électromagnétisme.
- 13 fiches de TD : TD1 exercices 1 à 4 ; TD2 exercices 1 à 6 ; TD3 exercice 5 ; TD4 exercices 1 et 4.
- 56 questions interactives : QCM, vrai/faux, réponses multiples et calculs.
- 84 flashcards, recherche, progression locale et calculateur de budget optique.
- Documents PDF et schémas fournis, accessibles depuis le site.

## Mettre le site sur GitHub Pages

1. Décompresse `Site_revision_Telecom3_GitHub.zip`.
2. Crée un dépôt GitHub, puis ajoute **tout le contenu décompressé** à la racine du dépôt. `index.html` doit être à la racine, avec `app.js`, `content.js`, `styles.css`, `assets/` et `sources/`. Ne dépose pas seulement le ZIP.
3. Dans le dépôt, ouvre **Settings → Pages**.
4. Sous **Build and deployment**, choisis **Deploy from a branch**.
5. Choisis la branche **main**, le dossier **/(root)**, puis **Save**.
6. Une fois la publication terminée, GitHub affiche l’adresse du site dans cette page.

Le fichier `.nojekyll`, inclus, indique qu’il s’agit de fichiers statiques déjà prêts. Aucun outil de compilation, aucune clé API et aucun serveur applicatif ne sont nécessaires. Tous les liens sont relatifs : le site fonctionne aussi dans un sous-dossier de dépôt GitHub Pages.

Documentation officielle de la procédure :
https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Utilisation locale

Ouvre `index.html` dans ton navigateur. Le contenu et les interactions ne nécessitent aucun téléchargement de dépendance. Pour un comportement de stockage local plus prévisible, sers le dossier avec un serveur HTTP local, par exemple `python -m http.server 8000`, puis ouvre `http://localhost:8000`.

La progression appartient au navigateur et à l’adresse utilisée. Elle n’est pas synchronisée entre appareils, ni entre la version Sites et GitHub Pages. La session de quiz en cours est conservée seulement jusqu’au rechargement de la page ; les chapitres révisés, cartes maîtrisées et meilleur score général sont sauvegardés localement.

## Modifier le site

- `index.html` : structure de la page et métadonnées.
- `styles.css` : présentation et adaptation aux écrans.
- `content.js` : fiches, TD, questions, tableaux complémentaires.
- `app.js` : navigation, recherche, quiz, flashcards, progression et calculateur.
- `assets/` : schémas fournis ou calculés.
- `sources/` : PDF du cours, des TD et de la documentation.

## Provenance et conventions

Source prioritaire : les deux PDF contenus dans le ZIP séparé `RT2-Telecom3-TD-26-27.zip` (cours complet annoté et TD avec annexes modifiées). Le ZIP principal apporte la documentation Amphenol, Infractive, le poster OTDR et les fiches constructeur. Les nouveaux ZIP portant `(1)` étaient identiques aux versions initiales. La capture `image(7).png` est également utilisée.

Les références de page sont des pages PDF, pas des numéros de diapositives. Le site distingue synthèse du support, correction pédagogique proposée et complément. Il ne prétend pas reproduire un corrigé officiel.

Conventions importantes : pertes positives en dB ; puissances en W ou dBm ; ouverture numérique sans unité ; angles mesurés à la normale. Le nombre de soudures et le sens de transmission sont précisés comme hypothèses lorsque l’énoncé est ambigu. Le modèle de la liaison de 1000 km est un bilan de puissance pédagogique, pas une validation de système réel.

## Vérifications réalisées

- Syntaxe JavaScript vérifiée.
- 8 chapitres, 13 exercices, 56 questions et 84 flashcards.
- Contrôle des 56 bonnes réponses et de cas de réponse fausse, partielle ou invalide.
- Contrôle des fonctions de progression et du calculateur de budget.
- Génération de 82 vues et vérification des liens locaux.
- Vérification des formules, unités, conversions et résultats numériques principaux.

La vérification visuelle dans un navigateur et la validation des outils WebMCP dans un navigateur compatible n’étaient pas disponibles dans l’environnement de création. Les outils WebMCP facultatifs ne sont activés que si le navigateur les prend en charge ; le site n’en dépend pas.
