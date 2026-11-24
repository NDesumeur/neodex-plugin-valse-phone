# Valse

Un jeu de rythme à une seule touche, dans le ciel de nuit : le soleil et la lune tournent l'un autour de l'autre sur un chemin de dalles. Au moment où l'astre qui tourne touche la dalle suivante, tape : il se pose, et c'est l'autre qui se met à tourner. Le chemin est dessiné par la musique. Joue les 1200 morceaux du plugin Rythme, ou ta propre musique.

*English version: [README.en.md](README.en.md)*

## Version téléphone

On joue d'un doigt : touche l'écran pile quand l'astre arrive sur la dalle dorée. Toucher le jeu lance le morceau en plein écran ; pendant la partie, le bouton PAUSE est posé en haut à droite du jeu (il reste là en plein écran), et le retour du téléphone met aussi en pause. Après une chute, toucher reprend au drapeau et le bouton DÉBUT repart du début. La partie se met en pause toute seule quand tu quittes l'appli. Le décalage se règle tout seul après chaque partie, utile car le son d'un téléphone arrive parfois un peu en retard.

## Comment jouer

- **N'importe quelle touche** (lettres, flèches, Entrée) ou un **clic** : poser l'astre sur la dalle dorée, pile au moment où il la touche.
- **Lire le chemin** : l'astre tourne d'un demi-tour par temps. Une **ligne droite** dure donc un temps, un **virage à angle droit** un demi-temps, un **virage serré** un quart de temps.
- **Trois points bleus** sur une dalle : l'astre y tourne plus lentement (une longue pause dans la musique).
- **Une boucle rose** : l'astre change de sens de rotation.
- **Trop tôt ou trop tard, c'est perdu** : seule la prochaine dalle compte, et un appui en trop pendant le temps qui la précède perd la partie. Taper au hasard ne marche donc pas. Deux touches presque ensemble (moins de 60 ms) ne comptent qu'une fois.
- **Drapeaux** : toutes les 32 dalles. Après une partie perdue, **Espace** reprend au dernier drapeau passé (sans record), **R** recommence depuis le début.
- La caméra suit l'astre, le ciel ne bouge pas : rien ne gêne la lecture du chemin.
- **Espace** : jouer · **P** : pause · **Plein écran** pendant la partie.

## Précision et points

Les notes sont jugées selon l'écart avec le bon moment : **Parfait** (environ ±45 ms), **Bien** (±90 ms), **OK** (±140 ms), sinon raté.

Les points d'une note augmentent de 1 % par note de combo, jusqu'au double à 100 notes de suite ; une note ratée remet le combo à zéro. À la fin, la précision donne une note : **S** à partir de 95 %, **A** à 90 %, **B** à 80 %, **C** à 70 %, **D** en dessous.

## Chansons et difficulté

L'onglet **Chansons** reprend les 1200 morceaux de Rythme, en quatre difficultés (Facile, Normal, Difficile, Expert). La difficulté de chaque niveau est calculée d'après ses notes (densité, passages chargés), de 1 à 10 étoiles.

## Mes musiques

Dans **Mes musiques**, crée un niveau à partir d'un **fichier audio** importé ou d'une musique de ta bibliothèque **NeoMusic** : le jeu trouve son tempo et ses temps forts et en fait un niveau, à la **difficulté** choisie (1 à 10 étoiles).

## Entraînement et figure

- **Départ** (entraînement) : commence à 25, 50 ou 75 % du morceau pour travailler un passage. Les notes d'avant ne comptent pas, et rien n'est gardé comme record.
- **Avancée** : quand tu perds, l'écran donne la part du morceau atteinte, et ton record sur ce niveau.
- L'écran de fin montre aussi **la figure dessinée par tout le chemin**, dalles réussies en vert et ratées en rouge.

## Réglages

- **Volume** de la musique.
- **Son des clics** : le son joué à chaque note touchée, au choix parmi 10 (Doux, Clap, Bois, Grosse caisse, Cristal, Pop, Charleston, Caisse claire, Pluck, Tok) ou aucun. Perdre un combo de 10 ou plus joue un son « combo cassé ».
- **Décalage** (−300 à +300 ms) : il se règle tout seul après chaque partie selon ton retard ou ton avance moyens ; tu peux aussi le changer à la main.

## Données et synchronisation

Tes scores et notes par niveau et tes réglages sont enregistrés par NeoDex, sauvegardés et synchronisés entre tes PC si la synchro est activée.

## Installer

Dans NeoDex : **NeoStore → À découvrir → Valse → Installer**.

Développer un plugin : voir le [SDK NeoDex](https://github.com/NDesumeur/neodex-sdk).

## Nouveautés de la version 2.0.0

- Le jeu est refait autour d'un jugement strict : trop tôt ou trop tard, la partie est perdue (avant, on pouvait taper au hasard et finir quand même).
- Drapeaux de reprise toutes les 32 dalles.
- Plus d'effets de caméra (zooms, rotations) ni de ciel qui défile : seul le chemin bouge.

## Nouveautés de la version 1.1.0

- **Manette** : la croix, A, B, X, Y et les gâchettes hautes posent l'astre ; Start lance le morceau (A aussi, hors partie) ; Select met en pause.
- **Courbe de précision** sur l'écran de fin : ta justesse tout au long du morceau, avec les notes ratées marquées en rouge dessous, pour voir où tu as décroché.
