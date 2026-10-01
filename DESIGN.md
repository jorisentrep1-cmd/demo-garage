---
name: Garage Viallard
description: Le site d'un garage de réseau, fait au niveau des meilleurs — clair, rassurant, prix et rendez-vous toujours visibles.
colors:
  fond: "#FFFFFF"
  fond2: "#F2F5F9"
  carte: "#FFFFFF"
  trait: "#DCE3EB"
  encre: "#0F1B2D"
  texte: "#364253"
  doux: "#566273"
  marque: "#0D3D82"
  bande: "#0D3D82"
  sur-bande: "#FFFFFF"
  sur-bande-doux: "#C8D5EA"
  jaune: "#FFC72C"
  jaune-survol: "#F2B600"
  sur-jaune: "#14140F"
  focus: "#1D63CF"
  puce-fond: "#FFEFC2"
  puce-texte: "#14140F"
typography:
  display:
    fontFamily: "'Barlow Semi Condensed', 'Barlow', sans-serif"
    fontSize: "clamp(2.5rem, 5.2vw, 4.4rem)"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "-.02em"
  headline:
    fontFamily: "'Barlow Semi Condensed', 'Barlow', sans-serif"
    fontSize: "clamp(1.85rem, 3.3vw, 2.6rem)"
    fontWeight: 700
    lineHeight: 1.08
    letterSpacing: "-.015em"
  title:
    fontFamily: "'Barlow Semi Condensed', 'Barlow', sans-serif"
    fontSize: "1.25rem"
    fontWeight: 700
    lineHeight: 1.08
    letterSpacing: "-.01em"
  price:
    fontFamily: "'Barlow Semi Condensed', sans-serif"
    fontSize: "1.55rem"
    fontWeight: 700
    lineHeight: 1
    fontFeature: "tnum"
  lead:
    fontFamily: "'Barlow', system-ui, sans-serif"
    fontSize: "1.12rem"
    fontWeight: 400
    lineHeight: 1.55
  body:
    fontFamily: "'Barlow', system-ui, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "'Barlow', system-ui, sans-serif"
    fontSize: ".88rem"
    fontWeight: 600
    lineHeight: 1.4
rounded:
  sm: "8px"
  md: "10px"
  lg: "12px"
  xl: "16px"
  pill: "999px"
spacing:
  gutter: "1.5rem"
  gutter-mobile: "1rem"
  container: "1240px"
  section: "5rem"
  section-mobile: "3.6rem"
  bloc: "2.4rem"
components:
  button-rdv:
    backgroundColor: "{colors.jaune}"
    textColor: "{colors.sur-jaune}"
    rounded: "{rounded.md}"
    padding: ".85rem 1.3rem"
  button-rdv-hover:
    backgroundColor: "{colors.jaune-survol}"
  button-contour:
    backgroundColor: "{colors.carte}"
    textColor: "{colors.encre}"
    rounded: "{rounded.md}"
    padding: ".85rem 1.3rem"
  button-contour-hover:
    textColor: "{colors.marque}"
  button-marque:
    backgroundColor: "{colors.bande}"
    textColor: "{colors.sur-bande}"
    rounded: "{rounded.md}"
    padding: ".85rem 1.3rem"
  nav-link:
    textColor: "{colors.texte}"
    typography: "{typography.label}"
    rounded: "{rounded.sm}"
    padding: ".5rem .55rem"
  nav-link-hover:
    backgroundColor: "{colors.fond2}"
    textColor: "{colors.encre}"
  badge:
    backgroundColor: "{colors.fond2}"
    textColor: "{colors.encre}"
    rounded: "{rounded.pill}"
    padding: ".3rem .7rem"
  badge-adaptable:
    backgroundColor: "{colors.puce-fond}"
    textColor: "{colors.puce-texte}"
    rounded: "{rounded.pill}"
    padding: ".3rem .7rem"
  card:
    backgroundColor: "{colors.carte}"
    rounded: "{rounded.xl}"
    padding: "1.8rem 1.6rem"
  question:
    backgroundColor: "{colors.carte}"
    textColor: "{colors.encre}"
    rounded: "{rounded.lg}"
    padding: "1.1rem 1.2rem"
---

# Design System: Garage Viallard

## Overview

**Creative North Star: « Le comptoir du garage de réseau »**

Le standard de la catégorie, assumé et tenu au niveau des meilleurs (AD, Eurorepar, Top Garage) : surfaces blanches et gris acier très clair, un bleu de marque profond, un jaune signal pour l'action. Rien ne cherche à surprendre dans la forme ; ce qui distingue le garage tient au fond, et le système est construit pour que ce fond se lise : les prix en chiffres tabulaires, le « non compris » écrit sous chaque forfait, l'écart origine/adaptable dans un tableau.

La densité est celle d'un site de service : titres courts en Barlow Semi Condensed, casse normale partout, texte courant en Barlow sur une base de lecture de 17 px. La profondeur vient d'ombres douces décalées vers le bas et de l'alternance blanc / gris acier entre sections ; le bleu ne remplit que les bandes de marque (contact) et les petites marques d'accent. Le seul mouvement est l'en-tête collant qui se resserre au défilement.

Le système refuse l'atelier noir et rouge en capitales et les grilles de cartes « icône + titre » empilées : les forfaits sont des lignes, pas des cartes.

**Key Characteristics:**
- Fond clair, bleu Viallard en accent et en bande, jaune réservé à l'action rendez-vous / appel.
- Barlow Semi Condensed 700 pour les titres et les prix, Barlow pour le reste ; jamais de capitales forcées.
- Chiffres tabulaires sur tout ce qui se compare (prix, écarts, horaires, téléphone, note).
- Coins francs mais adoucis (8 à 16 px), ombres douces décalées, filets de 1 px.
- Icônes SVG au trait 1,75, couleur héritée.
- Thème clair et thème sombre complets, contraste AA dans les deux.

## Colors

Une palette de garage de réseau : neutres bleutés très clairs, un bleu profond porteur de la marque et un jaune signal rare.

### Primary
- **Bleu Viallard** (`marque`, `bande`) : couleur de marque. `marque` colore les liens, les icônes d'accent (repères, forfaits, horaires), les prix et le lien de navigation actif (sur un fond à 10 % de mélange). `bande` remplit les surfaces de marque : bande contact, sigle « GV », bouton « Laisser un avis Google ». En clair les deux valent le même bleu ; en sombre ils se séparent (voir plus bas).

### Secondary
- **Jaune signal** (`jaune`, survol `jaune-survol`, texte posé dessus `sur-jaune`) : la couleur de l'action. Bouton « Prendre rendez-vous », pastille de la promesse d'appel, étape clé « On vous appelle » du déroulé, icônes et survol du téléphone sur la bande bleue, sélection de texte, lien d'évitement. Toujours avec `sur-jaune` quasi noir dessus, jamais du blanc.
- **Puce adaptable** (`puce-fond`, `puce-texte`) : jaune pâle pour le badge « 30 à 50 % moins cher » de l'option adaptable ; la seule autre teinte chaude du système.

### Neutral
- **Blanc** (`fond`, `carte`) : fond de page et surfaces de carte.
- **Gris acier très clair** (`fond2`) : sections alternées, barre d'infos, survols, pied du comparatif.
- **Filet acier** (`trait`) : tous les filets de 1 px, bords de contour, séparateurs de lignes et de colonnes.
- **Encre marine** (`encre`) : titres, valeurs en gras, texte sur cartes.
- **Ardoise** (`texte`) : texte courant.
- **Ardoise douce** (`doux`) : texte secondaire, mentions « dès », « non compris », horaires fermés.
- **Bleu clair sur bande** (`sur-bande-doux`) et **blanc sur bande** (`sur-bande`) : texte courant et titres posés sur la bande bleue.
- **Bleu focus** (`focus`) : contour de focus 3 px et curseur de saisie.

### Thème sombre
Bascule par `prefers-color-scheme` ou `data-theme="dark"` (deux blocs identiques sur `:root`). Valeurs : `fond` #0D131B, `fond2` #131B26, `carte` #17212E, `trait` #273445, `encre` #F1F4F8, `texte` #C3CCD8, `doux` #98A4B5, `marque` et `focus` #9DC1FA, `bande` #123A72, `puce-fond` rgba(255,199,44,.16), `puce-texte` #FFD45E. Le jaune du bouton ne change pas. En sombre les cartes reçoivent un bord `trait` (`--bord-carte`) et les ombres passent au noir pur.

### Châssis NovaSpot
Le bandeau « Exemple » garde en dur #0F1B2D et texte #E6EBF2 dans les deux thèmes : c'est le châssis commun aux six démos, pas une couleur du garage. Les étoiles de note sont en dur à #E8A400, décoratives (masquées aux lecteurs d'écran, la note est écrite à côté).

### Named Rules
**La règle du jaune qui appelle.** Le jaune ne marque que l'action rendez-vous / appel et ce qui la promet (pastille d'appel, étape « On vous appelle », téléphone sur la bande). Il n'est jamais un fond décoratif de section ni une couleur de titre.

**La règle des deux bleus.** `marque` est un bleu de texte et d'accent ; `bande` est un bleu de surface. En sombre, `marque` s'éclaircit pour rester lisible sur fond sombre tandis que `bande` reste profond : ne jamais utiliser l'un à la place de l'autre.

## Typography

**Display Font:** Barlow Semi Condensed 700 (repli Barlow, sans-serif)
**Body Font:** Barlow 400 / 500 / 600 / 700 (repli system-ui, sans-serif)

Toutes deux auto-hébergées dans `/fonts/`, sous-ensemble latin, `font-display: swap`. Base : `html` à 106,25 % (1 rem = 17 px), texte courant à 16 px.

**Character:** Une grotesque industrielle de signalétique, condensée pour les titres et les prix, pleine largeur pour le texte : sérieux de garage de réseau, sans dureté d'atelier.

### Hierarchy
- **Display** (700, clamp(2.5rem, 5.2vw, 4.4rem), 1) : titre d'ouverture uniquement ; un mot peut passer en `marque` sans italique (`em` en style normal). 2,35rem sous 560 px.
- **Headline** (700, clamp(1.85rem, 3.3vw, 2.6rem), 1,08) : titres de section, en tête d'un chapeau de 44rem maximum.
- **Title** (700, 1,2 à 1,45rem, 1,08) : titres de forfait, d'étape, d'option, de bloc horaires.
- **Price** (Semi Condensed 700, 1,55rem, 1, tabulaire) : prix des forfaits en `marque`, préfixe « dès » en Barlow 500 0,78rem `doux`. Les grands chiffres (note 3,6rem, téléphone de contact clamp(2.1rem, 4.4vw, 3.2rem)) suivent la même voix.
- **Lead** (400, 1,12rem, 1,55) : sous-titre d'ouverture, 34rem max ; chapeaux de section à 1,04rem.
- **Body** (400, 16px, 1,6) : texte courant ; dans les blocs 0,94 à 0,95rem.
- **Label** (600, 0,88rem) : navigation, liens d'en-tête, mentions secondaires de 0,78 à 0,9rem en `doux`.

### Named Rules
**La règle de la casse normale.** Aucun `text-transform` dans le système : titres, boutons, badges et étiquettes s'écrivent en casse de phrase.

**La règle du chiffre aligné.** Tout chiffre qui se compare ou se compose (prix, écarts, horaires, téléphone, note) porte `font-variant-numeric: tabular-nums` (classe utilitaire `.num` hors composants).

## Layout

Conteneur centré de 1240px avec gouttière de 1,5rem (1rem sous 560 px). Les sections respirent à 5rem verticalement (3,6rem sous 560 px), en alternant fond blanc et section `fond2`. Un chapeau de section (titre + paragraphe) tient dans 44rem ; les blocs de contenu commencent 2,2 à 2,6rem dessous.

Grilles asymétriques à deux colonnes pour les compositions mixtes (ouverture 1,05fr / 0,95fr, comparatif 1,6fr / 1fr, contact 1,1fr / 0,9fr), grilles régulières pour les séries (repères en 4, forfaits en 2 avec sous-grille de trois rangées pour aligner titres, textes et « non compris », déroulé en 4). Écarts de 2 à 3,5rem entre colonnes.

Paliers : 1140 px (la navigation disparaît, téléphone et rendez-vous restent), 900 px (tout passe à une colonne ou à deux pour les séries), 560 px (mobile : une colonne, boutons pleine largeur partagée, en-tête 3,9rem). L'en-tête collant mesure 4,6rem ; `scroll-padding-top` 5,5rem. Le bouton de rendez-vous abrège son libellé au lieu de disparaître (« Rendez-vous », puis « RDV » sous 380 px).

**La règle du pouce.** Téléphone et rendez-vous restent dans l'en-tête collant à toutes les largeurs.

## Elevation & Depth

Système hybride : à plat par défaut, séparé par filets et alternance de fonds ; les ombres sont douces, décalées vers le bas avec un étalement négatif, et réservées à ce qui se pose sur autre chose. En sombre, les mêmes ombres passent en noir plus dense et les cartes reçoivent un bord `trait`.

### Shadow Vocabulary
- **Ombre** (`--ombre` : `0 10px 28px -14px rgba(15,27,45,.28), 0 2px 6px -2px rgba(15,27,45,.08)`) : cartes posées sur la page (comparatif, note).
- **Ombre haute** (`--ombre-haute` : `0 18px 40px -18px rgba(15,27,45,.38), 0 3px 8px -3px rgba(15,27,45,.12)`) : étiquettes posées sur une photo (promesse d'appel, légende de bande photo).
- **Ombre bouton** (`--ombre-bouton` : `0 4px 12px -6px rgba(15,27,45,.35)`) : bouton jaune seulement.
- **Ombre d'en-tête** (`--ombre-entete` : `0 8px 24px -18px rgba(15,27,45,.5)`) : apparaît quand l'en-tête se resserre.

### Named Rules
**La règle de l'étiquette posée.** Une ombre haute signale un élément posé sur une photo ; une ombre simple une carte posée sur la page. Les lignes de tarifs, les repères et les questions n'ont pas d'ombre.

## Shapes

Coins adoucis, jamais ronds ni vifs : 8px pour les petits éléments interactifs (liens de navigation, lien d'évitement), 10px pour les boutons et contrôles d'en-tête, 12px pour les étiquettes et pavés d'icône, 16px pour les photos et grandes cartes. Pilule (999px) pour les badges, cercle pour les pastilles et numéros d'étape. Les bords sont des filets de 1 px `trait` (1,5px transparent sur les boutons pour qu'un contour n'ait pas de saut de taille ; 2px sur les numéros d'étape et la ligne du déroulé). Les photos sont recadrées en `object-fit: cover` avec un point focal explicite.

Icônes : SVG au trait (`stroke-width` 1,75, extrémités et jonctions arrondies, sans remplissage), 1,25em par défaut, couleur héritée ; seules les étoiles sont pleines.

## Components

### Buttons
Francs et lisibles, avec une hiérarchie stricte : un seul jaune.
- **Shape:** coins de 10px, Barlow 700 0,95rem, icône au trait à gauche, `padding` .85rem 1.3rem (1rem 1.5rem dans l'ouverture).
- **Rendez-vous (primaire) :** fond `jaune`, texte `sur-jaune`, ombre bouton ; survol `jaune-survol`, appui `translateY(1px)`.
- **Contour (secondaire) :** fond `carte`, bord 1,5px `trait`, texte `encre` ; au survol bord et texte passent en `marque`. Porte le numéro de téléphone ou l'action alternative.
- **Marque :** fond `bande`, texte blanc ; survol à 86 % mélangé de noir. Pour une action de marque hors rendez-vous (avis Google).
- **Hover / Focus :** transitions de 0,2s ; focus global : contour 3px `focus`, décalage 3px (contour jaune sur la bande bleue).

### Chips
- **Style :** badge pilule, 0,8rem 700, `fond2` / `encre` par défaut ; variante adaptable `puce-fond` / `puce-texte`.

### Cards / Containers
- **Corner Style :** 16px (12px pour les questions).
- **Background :** `carte` ; pied de comparatif en `fond2`.
- **Shadow Strategy :** Ombre simple (voir Elevation & Depth) ; bord `--bord-carte` transparent en clair, `trait` en sombre.
- **Internal Padding :** 1,8rem 1,6rem (1,5rem 1,3rem sous 600 px).

### Navigation
En-tête blanc translucide (94 % de `fond`, flou 10px), collant. Sigle « GV » sur carré `bande` de 2,3rem, nom en Semi Condensed 1,3rem. Liens en Label `texte`, survol fond `fond2`, actif en `marque` sur fond `marque` à 10 %. À droite : bascule de thème (carré de 2,4rem à bord `trait`), téléphone en gras avec icône `marque`, bouton jaune. Au défilement l'en-tête remonte de 0,45rem et gagne un filet et l'ombre d'en-tête (0,4s, `cubic-bezier(.16,1,.3,1)`), sans recalcul de mise en page.

### Grille tarifaire (signature)
Des lignes, pas des cartes : deux colonnes séparées par des filets `trait` en haut de chaque ligne. Chaque ligne : pavé d'icône 2,9rem à coins 12px (fond `marque` à 10 %, icône `marque`), titre, prix aligné à droite en Price, ce qui est compris, puis « Non compris : » en `doux` précédé d'un tiret au trait. Sous 480 px le prix passe sous le titre, aligné à gauche.

### Comparatif origine / adaptable (signature)
Carte unique à deux colonnes séparées d'un filet, chaque option avec titre, badge et texte ; pied pleine largeur sur `fond2` avec un tableau d'écarts (libellé à gauche, montant en gras tabulaire à droite, filets entre lignes).

### Étiquette posée
Carte `carte` à coins 10 à 12px avec ombre haute, posée sur le bas d'une photo (promesse d'appel avec pastille jaune ronde, légende de bande photo avec icône `marque`). Sous 900 / 620 px elle quitte la position absolue et chevauche le bas de la photo par une marge négative.

### Questions
`details` à fond `carte`, bord `trait`, coins 12px ; question en 700 `encre` 1,02rem, chevron au trait `doux` qui pivote de 180° (0,3s) ; survol en `marque`.

### Déroulé
Numéros en cercle de 2,7rem bordés de 2px `trait`, reliés par une ligne de 2px ; l'étape clé est pleine de `jaune`. Sous 560 px la ligne devient verticale.

## Do's and Don'ts

### Do:
- **Do** réserver `jaune` au rendez-vous, à l'appel et à ce qui les promet, toujours avec `sur-jaune` dessus.
- **Do** écrire les prix en Barlow Semi Condensed 700 tabulaire et dire ce qu'ils ne comprennent pas sur la même ligne.
- **Do** utiliser `marque` pour le texte et les accents, `bande` pour les surfaces bleues.
- **Do** garder téléphone et rendez-vous dans l'en-tête collant à toutes les largeurs, quitte à abréger le libellé.
- **Do** dessiner les icônes en SVG au trait 1,75, couleur héritée.
- **Do** vérifier chaque nouvelle couleur dans les deux thèmes ; une carte en sombre prend un bord `trait`.

### Don't:
- **Don't** forcer les capitales (`text-transform`) sur un titre, un bouton ou une étiquette.
- **Don't** composer l'atelier noir et rouge, ni empiler des cartes « icône + titre » : les forfaits sont des lignes.
- **Don't** mettre une ombre sur une ligne de liste, un repère ou une question ; l'ombre signale un élément posé.
- **Don't** poser du texte blanc sur le jaune.
- **Don't** utiliser d'emoji ou d'icônes pleines (hors étoiles de note).
