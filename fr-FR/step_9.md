## Événements

Voici les blocs dans la catégorie `Evénements`{:class="block3events"} lorsque les scripts sont démarrés.

Les **blocs en forme de chapeau** exécutent les blocs situés au dessous d'eux lorsqu'un événement particulier se produit. Ils sont arrondis au sommet, comme un chapeau, de sorte qu'aucun bloc ne peut être accroché au-dessus d'eux.

Tu peux utiliser:

```blocks3

when flag clicked // exécuter des blocs lorsque le drapeau vert au-dessus de la Scène est cliqué

when this sprite clicked // exécuter les blocs lorsque le sprite de ce script est cliqué

when stage clicked // exécuter les blocs lorsque la scène est cliquée

```

**Astuce :** Le bloc `quand la scène est cliquée`{:class="block3events"} n'est disponible que lorsque tu travailles dans la zone Code de la scène.

Si tu es sur un ordinateur avec un clavier, tu peux utiliser `quand la touche est pressée`{:class="block3events"} :

```blocks3
when [space v] key pressed // changer pour les touches numériques, alphabétiques ou fléchées
```

Tu peux également utiliser un bloc `quand l'arrière-plan bascule sur`{:class="block3events"} pour démarrer un script lorsque l'arrière-plan change.

[[[scratch3-changing-backdrops-pages-levels]]]

[[[scratch3-show-hide-sprites-backdrops]]]


Le bloc `quand >`{:class="block3events"} a deux versions :

```blocks3
when [loudness v] > (10) // exécuter des blocs lorsque le microphone détecte un son

when [timer v] > (10) // exécuter des blocs lorsque le chronomètre atteint 10 secondes
```

[[[scratch3-time-delay]]]


Les deux derniers blocs de la catégorie `événements`{:class="block3events"} sont `envoyer à tous`{:class="block3events"}. Tu peux utiliser `quand je reçois (message v)`{:class="block3events"} pour démarrer un script lorsqu'un sprite exécute un `envoyer à tous (message v)`{:class="block3events"} correspondant.

[[[generic-scratch3-broadcast-message]]]

