# Swiss Graphic Services

Site en français inspiré de l'identité d'origine : vrai logo SGS, noir, blanc, or et typographie Oswald. Photographies et vidéo issues du site existant.

## Vercel

Importer le dépôt sous le nom `swissgraphicservices`, framework **Other**. La configuration du dépôt définit la commande `node scripts/build.mjs` et le dossier de sortie `dist`. Aucune dépendance à installer.

## Prévisualisation locale

1. `node scripts/build.mjs`
2. `python3 -m http.server 8000 --directory dist`
3. Ouvrir http://localhost:8000.

Les liens sans extension utilisent les clean URLs de Vercel. Avec le serveur Python, ouvrir les pages locales sous leur nom `.html`.

## Pages locales

16 pages HTML autonomes pour Lausanne, Renens, Crissier, Ecublens, Prilly, Pully, Lutry, Épalinges, Le Mont-sur-Lausanne, Romanel-sur-Lausanne, Cheseaux-sur-Lausanne, Cugy, Morrens, Bottens, Échallens et Bretigny-sur-Morrens.

Chaque page comporte un titre, une description, un H1, un angle de contenu spécifique, les informations de l'atelier, un itinéraire, des liens internes et un formulaire de contact. Toutes indiquent le seul atelier réel à Bretigny-sur-Morrens. Aucun établissement secondaire ni temps de trajet n'est inventé.

Le build génère `sitemap.xml`, `robots.txt`, les URL canoniques et les métadonnées sociales. Le domaine est pris dans `SITE_URL` (si défini), sinon dans `VERCEL_PROJECT_PRODUCTION_URL`, puis `VERCEL_URL`. Si vous ajoutez un domaine personnalisé, définir `SITE_URL` dans Vercel et redéployer pour conserver un seul domaine canonique. En local, le domaine de sortie est http://localhost:8000.

## Contact et médias

Le formulaire prépare un message WhatsApp que le visiteur relit et envoie. Il ne stocke aucune donnée et ne prétend pas qu'un message a déjà été envoyé. Les photos WebP, le logo et la vidéo MP4 sont inclus dans `assets/`. La simulation 3D de l'accueil est identifiée comme telle.

## Vérification

Build statique, syntaxe JavaScript, structure des pages, ancres, liens internes, présence des médias, métadonnées uniques et sitemap vérifiés. Le rendu visuel et les interactions n'ont pas été vérifiés dans un navigateur dans cet environnement.
