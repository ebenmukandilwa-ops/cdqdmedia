# CDQD Média — site statique

Site 100 % statique : aucun serveur, aucune base de données. Il suffit de mettre le contenu de ce dossier à la racine de l’hébergement.

## Mise en ligne
- **Netlify** (gratuit) : app.netlify.com/drop, glissez le dossier.
- **Cloudflare Pages / Vercel / GitHub Pages** : déposez le dossier tel quel.
- **Hébergeur classique (cPanel, FTP)** : envoyez tout le contenu dans `public_html/` (le fichier `.htaccess` gère cache, compression et page 404).

## Avant la mise en ligne
Le domaine `https://cdqdmedia.com` est provisoire. Remplacez-le par votre vrai domaine dans :
`index.html` (balises canonical, og:url, og:image, JSON-LD), `robots.txt`, `sitemap.xml`.

## Ajouter une photo
1. Placez `NN.jpg` (pleine taille, max ~1600 px) et `NN-m.webp` (miniature 640 px) dans `images/`.
2. Copiez une ligne `<li data-cat="...">` dans `index.html` et adaptez le chemin, la légende et la catégorie (Mariage, Couple, Culte, Portrait, Design).

## Structure
index.html · 404.html · assets/style.css · assets/main.js · images/ · favicon.svg · icônes · site.webmanifest · robots.txt · sitemap.xml · .htaccess · _headers
