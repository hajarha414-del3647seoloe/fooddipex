# FOODIPEX — site vitrine

Site statique premium en français pour FOODIPEX, société casablancaise active dans l'import-export agricole. Il utilise uniquement HTML5, CSS3 et JavaScript natif, sans dépendance, police distante, cookie, suivi ou service tiers.

## Structure

- `index.html` : accueil, entreprise, activité, démarche, identité, FAQ et contact.
- `privacy-policy.html` : politique conforme au fonctionnement actuel.
- `404.html` : page d'erreur.
- `assets/css/` : design, animations et adaptations responsives.
- `assets/js/` : navigation, formulaire et animations.
- `assets/images/` : favicon et aperçu social SVG originaux.
- `robots.txt`, `sitemap.xml` : bases SEO à finaliser avec le domaine.

## Utilisation locale

Ouvrir `index.html` directement, ou lancer dans ce dossier `python -m http.server 8000`, puis ouvrir `http://localhost:8000`.

## Personnalisation

Les informations de société se trouvent dans `index.html`. Les couleurs sont au début de `assets/css/style.css`. Le monogramme CSS est temporaire : remplacez les blocs `.brand-mark` par une image lorsque le logo officiel sera fourni. Ajoutez les images dans `assets/images/`, avec des noms descriptifs, dimensions et textes alternatifs. Les activités sont les cartes de la section `#activite`.

Le formulaire valide les champs et copie un message dans le presse-papiers. Il n'envoie rien et ne simule pas une livraison. Pour un backend, remplacez ce comportement dans `assets/js/main.js` par un appel `fetch` HTTPS, protégez le point d'accès contre le spam, puis mettez à jour la politique. Pour l'e-mail ou WhatsApp, ajoutez uniquement des coordonnées professionnelles confirmées et utilisez respectivement `mailto:` ou `https://wa.me/` au format international.

Le site n'utilise aucun cookie : aucun bandeau n'est nécessaire. Si un outil d'analyse ou un contenu tiers est ajouté, bloquez-le avant consentement, fournissez Accepter/Refuser et mettez à jour la politique. Faites relire le texte légal par un professionnel qualifié avant publication. Configurez côté serveur HTTPS et une Content-Security-Policy adaptée.

## SEO et déploiement

Remplacer `example.com` dans `sitemap.xml` et `robots.txt`, ajouter les URL canoniques et remplacer l'aperçu social provisoire. Sur GitHub Pages, publier la branche via Settings > Pages. Sur Netlify ou Vercel, importer le dossier sans commande de build et utiliser `.` comme répertoire de publication. Sur un hébergement classique, transférer tout le contenu en conservant l'arborescence.

## Information required before production launch

- Domaine de production et URL canoniques
- Logo officiel, favicon et visuel social validé
- E-mail général et e-mail confidentialité
- Téléphone et numéro WhatsApp au format international
- Confirmation de l'adresse à publier (les sources D&B et fiscales diffèrent)
- Produits, marchés, zones desservies et photos autorisées
- Horaires et liens sociaux éventuels
- Représentant légal et coordonnées confidentialité, si publication souhaitée
- Hébergeur, localisation des serveurs et politique de journaux
- Backend du formulaire ou canal de contact retenu
- Choix analytique et exigences cookies, si ajout futur
- Domaine dans le sitemap et `robots.txt`
- Validation juridique de la politique

## Sources et hypothèses

Les fichiers fournis confirment : FOODIPEX, SARL, ICE `001524678000009`, RC/identifiant fiscal `116673`, D‑U‑N‑S® `659647420`, activité « import export, exportation », secteur agriculture et statut actif. L'adresse fiscale utilisée est `257/259, boulevard Abdelmoumen, Casablanca`; D&B indique séparément « Zone Technopole, aéroport Mohamed V ». Aucun produit, chiffre, témoignage, certification, contact, logo ou photo n'a été inventé. Le français a été retenu car les documents administratifs exploitables sont principalement en français.
