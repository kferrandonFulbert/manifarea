# agent.md — Instructions IA pour le blog Manifarea

Version : 30 octobre 2026. Langue : français de France.

## 1. Mission et périmètre

Créer et maintenir un blog éditorial consacré à **Manifarea**, en HTML, CSS et JavaScript. Livrer un site rapide, accessible, responsive et optimisé pour la recherche, avec des articles utiles, originaux et sourcés.

Le livrable est un blog autour du jeu, pas une réimplémentation du jeu. Ne pas développer de serveur multijoueur ni intégrer le jeu sans demande explicite. Préférer du HTML statique ; un générateur peut faciliter les gabarits si son résultat reste du HTML complet. Ne pas imposer de framework lourd.

## 2. Contexte fourni par le propriétaire

Ces éléments constituent le brief du projet, pas des faits vérifiés indépendamment :

- Le jeu s'appelle Manifarea et se déroule à Chartres.
- Il permet d'incarner des manifestants en rouge ou des CRS en bleu.
- Il utilise Three.js pour sa dimension graphique et WebSocket pour les échanges réseau. Employer les noms « Three.js » et « WebSocket », et non « treejs ».
- Il propose une satire de l'actualité française et permet d'en rire à travers un univers vidéoludique.
- Le blog traite du gameplay, des cheatcodes, du graphisme, de la technique, de la communauté, des mises à jour et des parallèles avec l'actualité.

Ne pas déduire du brief des règles, modes, cartes, lieux précis, commandes, objectifs, capacités, performances ou fonctionnalités absents des sources. Ne pas affirmer que la cathédrale ou un monument chartrain est visible sans preuve.

## 3. Vérifications avant réalisation

1. Lire les fichiers et consignes du dépôt existant ; conserver son organisation quand elle est pertinente.
2. Identifier l'URL du jeu, le domaine du blog, le statut officiel ou indépendant du blog, l'auteur réel, les contacts et les droits sur les médias.
3. Examiner les sources disponibles : jeu, documentation, code autorisé, annonces et notes de version.
4. Inventorier les informations confirmées et les points inconnus dans un document de travail.
5. Continuer les travaux indépendants des informations manquantes. Garder les pages non vérifiées en brouillon, hors sitemap et hors indexation.

Ne jamais inventer un domaine de production, un compte Discord, des statistiques, des joueurs, des témoignages, une équipe éditoriale, un accès au jeu ou une citation. Aucun lien « Jouer » ne doit mener vers une adresse supposée. Les valeurs de gabarit ne doivent pas subsister dans les pages publiées.

## 4. Ligne éditoriale

### Public et promesse

S'adresser aux joueurs débutants ou habitués, aux amateurs de jeux indépendants, aux curieux de Chartres et aux lecteurs intéressés par la satire française. Expliquer clairement, avec humour, comment découvrir le jeu et suivre son évolution.

### Ton

Français naturel, vivant, complice et légèrement irrévérencieux. Employer le tutoiement dans les guides. Conserver des explications factuelles précises et réserver les formulations les plus humoristiques aux introductions, légendes et encadrés. Éviter les titres trompeurs, les clichés répétés et les textes de remplissage.

Distinguer visuellement et explicitement : **fait vérifié**, **avis de la rédaction**, **fiction/satire** et **hypothèse**. Ne jamais présenter une blague ou une scène du jeu comme une information réelle.

Ne pas transformer les couleurs des équipes en jugement sur des personnes réelles. Pas de harcèlement, d'accusations non établies ou de fausses citations attribuées à des personnes identifiables. Les conseils de confrontation restent exclusivement des conseils de gameplay.

### Actualité française et parallèle satirique

Chaque article d'actualité distingue :

1. Le contexte réel, daté et relié à des sources fiables.
2. Le lien documenté avec le jeu ou, à défaut, une lecture personnelle explicitement présentée comme telle.
3. Le commentaire humoristique clairement identifiable.

Privilégier les sources primaires et recouper les affirmations sensibles. Ne pas prétendre qu'une mise à jour répond à un événement sans annonce du développeur. Indiquer la date de l'événement, pas seulement la date de publication. Corriger les erreurs de manière visible. Ne pas réécrire automatiquement toute l'actualité nationale pour attirer du trafic sans rapport avec Manifarea.

### Cheatcodes

Créer une rubrique dédiée, sans inventer de code. Pour chaque code confirmé : code exact, source, date du test, version du jeu, mode compatible, procédure et effet réellement observé, restrictions éventuelles. Identifier clairement les codes officiels, commandes de développement et éléments historiques.

Si aucun code n'est confirmé, l'indiquer ; ne pas publier une liste fictive pour capter une requête. Une page utile peut expliquer l'état des vérifications et orienter vers les commandes documentées. Ne pas fournir d'exploitation du serveur, de contournement anti-triche ou de procédé donnant un avantage non autorisé en multijoueur.

## 5. Architecture éditoriale et navigation

Structure indicative, à adapter aux contenus réellement disponibles :

```text
/
/decouvrir/
/gameplay/
/gameplay/debuter/
/gameplay/manifestants/
/gameplay/crs/
/cheatcodes/
/graphismes/
/technique/
/communaute/
/actualites/
/satire-et-actualite/
/a-propos/
/contact/
/mentions-legales/
/confidentialite/
```

Chaque rubrique doit apporter une vraie synthèse et des liens vers ses articles. Ne pas créer de catégories vides ou de multiples pages équivalentes. Prévoir une navigation principale courte, un fil d'Ariane sur les pages internes, des articles associés et un flux RSS si utile.

Une page peut être stockée sous `rubrique/slug/index.html` si l'hébergement sert ces chemins. Choisir une convention unique d'URL et de barre finale. Préserver les URL existantes ; mettre en place des redirections permanentes lors des changements.

## 6. Plan de contenus initial

Ces titres sont des pistes, pas des affirmations à publier sans recherche.

| Page ou sujet | Intention principale | Preuves nécessaires |
| --- | --- | --- |
| Manifarea : découvrir le jeu satirique situé à Chartres | Découverte du jeu | Sources du projet, captures autorisées |
| Débuter dans Manifarea : commandes et premières parties | Aide aux débutants | Commandes et déroulement vérifiés |
| Manifestants rouges et CRS bleus : comprendre les deux camps | Compréhension du gameplay | Différences et objectifs documentés |
| Cheatcodes Manifarea : codes confirmés et conditions d'utilisation | Recherche de codes | Codes sourcés et tests reproductibles |
| Chartres dans Manifarea : décor et interprétation artistique | Univers du jeu | Comparaisons visuelles vérifiables |
| Graphismes de Manifarea : direction artistique et lisibilité | Analyse visuelle | Captures et observations précises |
| Three.js et WebSocket : comprendre la technique de Manifarea | Compréhension technique | Documentation et, pour l'implémentation, code autorisé |
| Comment suivre les mises à jour de Manifarea | Actualité du jeu | Canaux authentifiés et notes de version |
| Communauté Manifarea : où échanger et proposer des idées | Participation | Liens et règles vérifiés |
| Quand Manifarea fait écho à l'actualité française | Analyse satirique | Événement sourcé, lien avec le jeu explicité |

Publier d'abord quelques articles solides, puis élargir selon les questions réelles des joueurs. Aucun quota de mots ni rythme de publication artificiel.

## 7. Charte graphique bleu, blanc, rouge

Créer une identité française, ludique et éditoriale, sans donner l'impression d'un service public ou d'un site officiel des forces de l'ordre.

```css
:root {
  --bleu-france: #000091;
  --blanc: #ffffff;
  --rouge-france: #e1000f;
  --texte: #161616;
  --fond: #f6f6f9;
  --bordure: #d8d8e5;
  --bleu-pale: #eeeeff;
  --rouge-pale: #fff0f1;
  --largeur-contenu: 74rem;
  --largeur-lecture: 70ch;
}
```

- Fond blanc ou légèrement grisé, texte foncé, bleu pour la structure et les liens, rouge pour les accents et le camp manifestant.
- Évoquer le drapeau par un liseré tricolore discret, des séparateurs ou des détails de cartes ; éviter les grands aplats fatigants.
- Identifier les camps avec un libellé ou un pictogramme en plus de la couleur.
- Typographie lisible, système ou police locale ; hiérarchie nette et corps de texte confortable.
- Accueil de magazine : une mise en avant principale, des articles récents, un accès aux guides et des rubriques lisibles.
- Pages d'article sobres : titre, résumé, métadonnées, image pertinente, sommaire si nécessaire, lecture sans surcharge.
- Captures authentiques avec légendes. Une illustration conceptuelle doit être présentée comme telle, jamais comme capture de gameplay.
- Animations légères et respect de `prefers-reduced-motion`. Aucun canvas ou effet 3D indispensable à la lecture.

## 8. HTML, accessibilité et comportement

Utiliser HTML sémantique : `header`, `nav`, `main`, `article`, `section`, `aside`, `footer`, avec un H1 principal et une hiérarchie H2/H3 cohérente. Définir `lang="fr"`, UTF-8 et la balise viewport.

Le contenu et les liens essentiels doivent être présents dans le HTML livré, lisibles sans JavaScript. Employer des liens `<a href>` pour naviguer et des boutons pour les actions. Ajouter un lien d'évitement, un focus visible, des libellés de formulaire et des messages d'erreur compréhensibles. Vérifier le clavier, le zoom, les contrastes WCAG AA et les formats mobiles.

Images informatives : texte alternatif descriptif. Images décoratives : `alt=""`. Définir leurs dimensions. Les menus mobiles et accordéons doivent annoncer leur état. Ne pas inventer une recherche, un formulaire de contact ou des commentaires fonctionnels si aucun mécanisme ne les traite. Un blog statique n'implique pas un serveur WebSocket.

Séparer les styles et scripts réutilisables, utiliser les modules JS si nécessaire et limiter les dépendances. Ne jamais exposer de secrets. Si un contenu communautaire est intégré, l'échapper ou l'assainir et encadrer sa modération.

## 9. SEO : socle applicable en 2026

### Contenu et intention

Attribuer une intention claire à chaque page, avec une expression principale et quelques variantes naturelles. « Manifarea » est l'orthographe de référence. Ne pas créer de pages quasi identiques pour les variantes ou fautes de frappe. Mettre rapidement à disposition la réponse attendue, puis les explications et preuves.

Favoriser les tests réellement réalisés, captures originales, observations concrètes et sources consultables. Ne jamais écrire « nous avons testé » sans test. Signer avec une personne ou une organisation réelle et relier à une présentation honnête. Ne pas inventer d'expertise ou de biographie. Une date de modification ne change qu'après modification substantielle.

### Métadonnées et indexation

- Un `title` descriptif et distinct par page, cohérent avec le H1. Viser la concision ; une longueur de caractères n'est pas une règle de classement.
- Une méta-description spécifique, utile et naturelle. Elle propose un extrait ; son affichage et son effet sur le trafic ne sont pas garantis.
- Une URL stable, courte et descriptive, en minuscules, avec tirets.
- Une canonique absolue et cohérente vers la véritable URL de référence ; ne pas canoniser tous les articles vers l'accueil.
- Métadonnées Open Graph et cartes sociales avec image pertinente et URL absolue. Elles servent au partage, sans promesse de gain de classement.
- Sitemap XML contenant uniquement les URL canoniques indexables publiées, en réponse HTTP 200. `lastmod` reflète les modifications réelles.
- `robots.txt` cohérent avec le site. Ne pas y bloquer une page dont le `noindex` doit être lu. Robots.txt ne protège pas des données privées.
- Prévoir les vrais statuts HTTP : 404 pour une page absente, 301/308 pour un déplacement permanent ; aucune fausse 404 en 200.
- Garder les brouillons en dehors de la production ou utiliser `noindex` lorsqu'ils doivent être accessibles ; retirer le `noindex` des pages publiques à indexer.
- Pas de méta `keywords`, texte caché, bourrage de mots-clés, liens achetés pour manipuler le classement ou pages générées en masse sans valeur ajoutée.

### Maillage et découverte

Relier chaque article à sa rubrique et à des contenus pertinents avec des ancres descriptives. Éviter les articles orphelins. Les pages paginées ont leurs propres URL et canoniques. Ne pas dépendre d'un défilement infini pour découvrir les articles.

Citer les sources externes utiles sans `nofollow` systématique. Identifier les liens sponsorisés avec `rel="sponsored"` et les liens de contributions utilisateurs avec `rel="ugc"` lorsque pertinent. Ne pas créer de faux profils locaux ni de balisage LocalBusiness uniquement parce que le jeu se déroule à Chartres.

### Données structurées

Produire du JSON-LD valide et cohérent avec les informations visibles :

- `BlogPosting` pour les articles ; `NewsArticle` seulement si le contenu relève réellement de l'information d'actualité.
- `BreadcrumbList` pour le fil d'Ariane.
- `WebSite` et `Organization` ou `Person` uniquement avec une identité réelle et vérifiée.
- Renseigner les propriétés pertinentes : `headline`, `description`, `image`, `author`, `datePublished`, `dateModified` et `mainEntityOfPage`.
- Dates ISO 8601 avec fuseau ; images et liens accessibles ; aucune fausse note ou statistique.

Ne pas promettre d'extraits enrichis. Ne pas ajouter du FAQPage dans l'espoir d'obtenir systématiquement un résultat enrichi. Valider selon les fonctionnalités réellement prises en charge par Google au moment de la mise en ligne.

### Recherche assistée par IA

Les fondamentaux SEO restent applicables : contenu textuel accessible, réponses précises, preuves, structure claire et cohérence des données structurées. Aucun balisage « IA » spécial ni fichier `llms.txt` n'est nécessaire pour apparaître dans les fonctionnalités IA de Google. Ne promettre ni citation par une IA ni indexation ni position dans les résultats.

### Performance

Viser les bons seuils Core Web Vitals au 75e percentile des visites : LCP ≤ 2,5 s, INP ≤ 200 ms et CLS ≤ 0,1. Les résultats de laboratoire aident au diagnostic ; ils ne remplacent pas les données de terrain.

Compresser les images, proposer AVIF/WebP avec repli adapté, `srcset` et `sizes`. Ne pas charger paresseusement l'image principale susceptible d'être le LCP ; réserver le lazy-loading aux médias hors écran. Réduire CSS et JS, différer les scripts non essentiels, mettre en cache les ressources versionnées et limiter les services tiers. Ne pas charger Three.js sur le blog seulement parce que le jeu l'utilise.

## 10. Gabarit éditorial d'un article

Chaque article publié comprend selon son sujet :

1. Titre précis et résumé répondant à l'intention.
2. Auteur réel, date de publication et éventuelle mise à jour justifiée.
3. Introduction contextualisée avec le niveau de vérification.
4. Développement structuré avec exemples, étapes ou comparaisons utiles.
5. Captures et légendes quand elles apportent une preuve ou une explication.
6. Encadré satire, technique ou avertissement de version si pertinent.
7. Sources datées et crédits des médias.
8. Liens vers les articles utiles et appel à l'action correspondant à un service réellement disponible.

Pour un guide, mentionner la version testée et les limites connues. Pour un article technique, distinguer l'explication générale de Three.js/WebSocket de ce que l'on sait effectivement de l'implémentation de Manifarea. Pour la communauté, demander l'accord avant de publier des informations personnelles et ne pas fabriquer de verbatims.

## 11. Livrables attendus de l'IA qui réalisera le site

- Pages HTML complètes, feuilles CSS partagées et JavaScript limité aux interactions utiles.
- Gabarits cohérents, navigation, 404 et fichiers d'indexation adaptés à l'hébergement.
- Images optimisées et crédits, avec droits établis.
- Articles réellement documentés ; brouillons identifiés pour les sujets restant à vérifier.
- Documentation de lancement, d'ajout d'article, de mise à jour du sitemap et de déploiement.
- Inventaire des sources, des éléments restant à confirmer et des contrôles exécutés.

Ne jamais déclarer une intégration, publication, mesure de terrain ou vérification réussie si elle n'a pas été réalisée. Ne pas déployer le blog à partir de ce seul document sans demande de réalisation ou de publication du propriétaire.

## 12. Contrôles avant livraison du site

- [ ] Identité, liens du jeu, fonctionnalités et cheatcodes vérifiés ou laissés en brouillon.
- [ ] Faits, commentaire et satire clairement distincts ; actualité sourcée et datée.
- [ ] Aucune valeur de démonstration, fausse citation ou statistique inventée.
- [ ] HTML valide ; navigation et contenus essentiels utilisables sans JavaScript.
- [ ] Mobile, clavier, focus, contraste et réduction des animations contrôlés.
- [ ] Titres, descriptions, canoniques, liens internes et statuts HTTP contrôlés.
- [ ] Sitemap et robots cohérents ; aucune page publique bloquée par erreur.
- [ ] JSON-LD validé avec Schema Markup Validator et, si applicable, Rich Results Test.
- [ ] Performance évaluée sur mobile avec Lighthouse ou PageSpeed Insights ; résultats consignés sans les présenter comme des mesures de terrain.
- [ ] Médias autorisés, optimisés et correctement légendés.
- [ ] Search Console configurée et sitemap soumis si les accès sont disponibles ; sinon indiquer cette action comme restant à effectuer.

Après publication, suivre les impressions, clics, requêtes et pages dans Search Console ainsi que les Core Web Vitals disponibles. Prioriser les mises à jour utiles ; aucune promesse de première position ou de volume de trafic.

## 13. Références et entretien des consignes

Références officielles consultées le 30 octobre 2026 ; vérifier leur état avant une future refonte :

- Contenu utile : https://developers.google.com/search/docs/fundamentals/creating-helpful-content?hl=fr
- Fonctionnalités IA et SEO : https://developers.google.com/search/docs/appearance/ai-features?hl=fr
- Articles et JSON-LD : https://developers.google.com/search/docs/appearance/structured-data/article?hl=fr
- Guide SEO : https://developers.google.com/search/docs/fundamentals/seo-starter-guide?hl=fr
- Core Web Vitals : https://web.dev/articles/vitals?hl=fr

Le terme « SEO 2026 » désigne l'application de recommandations vérifiées à cette date, pas l'existence d'une recette annuelle ou d'une garantie de classement.

## 14. Utilisation du fichier par les agents

Le nom demandé est `agent.md`. Tous les outils IA ne le découvrent pas automatiquement : le joindre explicitement au contexte ou indiquer son chemin. Pour les outils qui attendent `AGENTS.md`, le propriétaire peut le renommer ou reporter ces consignes dans le fichier attendu. Ne pas maintenir deux versions divergentes.
