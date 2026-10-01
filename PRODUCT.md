# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Deux publics, dans cet ordre d'importance :

1. **Le garagiste prospecté par NovaSpot** (artisan indépendant du Blayais, Gironde). Il découvre la démo
   soit au comptoir, sur le téléphone de Joris, soit plus tard sur son ordinateur via un lien envoyé.
   Les deux écrans comptent autant. Son travail : se projeter (« c'est mon garage, en mieux ») et décider
   s'il prend un site NovaSpot.
2. **L'automobiliste du coin**, client fictif du garage : il cherche un garage fiable près de chez lui,
   veut un prix et un numéro, souvent sur téléphone. Il arrive aussi par le QR code agrafé à la facture
   (section avis).

## Product Purpose

Site de démonstration d'un garage fictif, Garage Viallard à Saint-Savin, réalisé par NovaSpot. Il prouve à
un garagiste réel qu'un site peut parler de son métier mieux qu'un gabarit. Réussite : le garagiste
reconnaît son quotidien et demande le même.

## Positioning

Le garage montre ce qu'un gabarit ne peut pas inventer : il appelle avant toute réparation payante ; il
donne le prix de la pièce d'origine et celui de l'adaptable, avec l'écart chiffré ; chaque forfait dit ce
qu'il ne comprend pas ; il assume ses limites (pas centre de contrôle technique agréé).

## Operating Context

- Démonstration au comptoir, debout, sur téléphone, en quelques secondes ; puis relecture au bureau.
- Les clients du garage lisent sur téléphone, pas toujours avec de bons yeux : base de lecture 17 px,
  texte courant 16 px.
- Le site fait partie d'une série de six démos NovaSpot (bâtiment, coiffure, garage, jardinage, nettoyage,
  ostéopathie animale) qui partagent un châssis : bandeau « Exemple » en tête, barre d'accès collante avec
  le téléphone, bloc contact, pied de page avec la mention « Informations fictives ».

## Capabilities and Constraints

- HTML/CSS statique, une seule page, sans framework ni build ; JavaScript léger et facultatif (le site
  fonctionne sans). Hébergement Cloudflare Pages, `/img/*` servi en cache immuable un an : toute image
  modifiée change de nom.
- Bascule thème clair / sombre (stockée sous `ns-theme`), contraste AA vérifié dans les deux thèmes.
- `noindex,nofollow` : c'est une démo.
- Le lien d'avis Google garde le paramètre `PLACE_ID_DU_CLIENT` (remplacé pour un vrai client).
- Prix ancrés sur le marché local (Gironde rurale), pas sur les prix nationaux.
- Jamais de secteur CHR (restaurants, bars, cafés, hôtels, gîtes, chambres d'hôtes) dans les visuels ou textes.

## Brand Commitments

- Nom : Garage Viallard (vérifié sans homonyme en Gironde), 12 route de Bordeaux, 33920 Saint-Savin,
  05 57 00 00 01, depuis 2011.
- Ton : direct, au « on », phrases de comptoir (« Si ça sonne dans le vide, c'est qu'on est sous une voiture »).
- Pas d'emoji ; icônes SVG au trait.
- Le bandeau « Exemple — site de démonstration réalisé par NovaSpot » et la mention « Informations fictives »
  restent obligatoires.

## Evidence on Hand

- Contenu complet dans `index.html` : six forfaits avec prix et exclusions, origine/adaptable avec écarts
  (≈ 60 € sur un freinage, jusqu'à 300 € sur un embrayage), déroulé en quatre étapes, quatre questions de
  comptoir, horaires, note 4,7 sur 81 avis (fictive, démo).
- Photos (Unsplash) dans `img/` : voiture sur pont, plaque floutée (`g-atelier-flou*.jpg`, portrait) ;
  train avant sur chandelles (`g-dessous.jpg`) ; mécanicien sur moteur (`g-moteur.jpg`, portrait) ;
  main et clé dans le compartiment moteur (`g-cle.jpg`).
- Aucun vrai avis client, aucune vraie photo du garage : ne rien inventer qui se présente comme réel au-delà
  de la fiction déclarée de la démo.

## Product Principles

1. Prouver plutôt qu'affirmer : prix, exclusions et écarts chiffrés avant les adjectifs.
2. Le téléphone du garage est l'action principale, partout à portée de pouce.
3. Une limite assumée vaut mieux qu'une promesse de plus.
4. Lisible au comptoir en cinq secondes, convaincant au bureau en deux minutes.

## Accessibility & Inclusion

WCAG AA dans les deux thèmes (surfaces inversées comprises), texte courant 16 px minimum, cibles tactiles
confortables, `prefers-reduced-motion` respecté.
