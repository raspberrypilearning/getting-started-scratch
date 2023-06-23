## Mouvement

Les blocs `avance`{:class="block3motion"} vous permettent de déplacer votre sprite sur la scène.

### Mouvement

Le bloc `avance`{:class="block3motion"} est le moyen le plus simple pour commencer à déplacer un sprite :

```blocks3
move [10] steps
```

Tu peux `aller à`{:class="block3motion"} ou `glisser en`{:class="block3motion"} le pointeur de la souris, une position aléatoire sur la scène (ou votre doigt sur une tablette), ou un autre sprite :

```blocks3
go to (position aléatoire v)

glide [1] secs to (position aléatoire v)
```

Tu peux aussi `aller à`{:class="block3motion"} ou `glisser en`{:class="block3motion"} une position donnée par des coordonnées `x`{:class="block3motion"} et `y`{:class="block3motion"} sur la scène.

```blocks3
go to x: [0] y: [0] 

glide [1] secs to x: [0] y: [0]
```

[[[scratch3-glide-to-object]]]

**Astuce :** Lorsque tu fais glisser un sprite sur la Scène, les blocs de mouvement qui utilisent les coordonnées `x`{:class="block3motion"} et `y`{:class="block3motion"} sont mis à jour dans le menu `Mouvement`{:class="block3motion"}. Les coordonnées `x`{:class="block3motion"} et `y`{:class="block3motion"} sont affichées dans le volet Sprite.

### Rotation
Tu peux également changer la `direction`{:class="block3motion"} vers laquelle pointe un sprite. Cela change la direction dans laquelle le sprite se déplacera si tu utilises un bloc `avancer`{:class="block3motion"}. Cela peut également changer la rotation du costume du sprite en fonction du réglage `style de rotation`{:class="block3motion"}.

Lorsque tu ajoutes un sprite, il sera orienté vers la droite (90 degrés). Tu peux modifier cela dans le volet Sprite ou en utilisant des blocs de code.

```blocks3
turn right [15] degrees

turn left [15] degrees

point in direction [90] // Clique sur 90 et fais glisser la flèche pour changer

point towards (pointeur de souris v)

(direction)

set rotation style [gauche-droite v] // ou ne tourne pas ou 360°
```

[[[scratch3-sprite-direction]]]

[[[scratch3-left-right-direction]]]

--- collapse ---
---
title: Tournoyer
---

--- no-print ---

**La chauve-souris tournoyante** : [Voir à l'intérieur](https://scratch.mit.edu/projects/435704980/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435704980/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Ce code fait tourner un sprite lorsque le drapeau vert est cliqué :

```blocks3
when flag clicked
forever
turn right (1) degrees :: motion
```

Dans un boucle `tourner`{:class="block3motion"} placé dans une boucle `répéter indéfiniment`{:class="block3control"}, change le nombre de degrés à `1` et ton sprite tournera sur place.

**Astuce :** Si tu n'ajoutes pas de bloc `avancer`{:class="block3motion"}, ton sprite tournera sur place.

--- /collapse ---

--- collapse ---
---
title: Se déplacer en cercle
---

--- no-print ---

**Orbite lunaire** : [Voir à l'intérieur](https://scratch.mit.edu/projects/435701055/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435701055/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Ce code fait voler un sprite en rond lorsque l'on clique sur le drapeau vert :

```blocks3
when green flag clicked
forever
move (1) steps
turn right (1) degrees :: motion
```

Modifie les valeurs d'un bloc `avancer`{:class="block3motion"} et d'un bloc `tourner`{:class="block3motion"} placé dans un bloc `répéter indéfiniment`{:class="block3control"} à `1` et ton sprite semblera se déplacer en cercle.

**Astuce :** Si tu veux que ton sprite commence toujours au centre de la scène, tu peux ajouter un bloc `aller à x:`{:class="block3motion"} `0` `y:`{:class="block3motion"} `0` avant le bloc `répéter indéfiniment`{:class="block3control"}.

--- /collapse --- 

### Rebondir

Le bloc `rebondir si le bord est atteint`{:class="block3motion"} est vraiment utile lorsque tu veux faire rebondir un sprite et rester sur la Scène :

```blocks3
if on edge, bounce
```

Découvre quelques-unes des façons dont tu peux faire rebondir ton sprite :

--- collapse ---
---
title: Rebondir sur la scène
---

--- no-print ---

**Fille se déplaçant à travers la scène** : [Voir à l'intérieur](https://scratch.mit.edu/projects/433535326/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433535326/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Ce code fait rebondir un sprite sur les bords gauche et droit de la Scène. Étant donné que le sprite tourne horizontalement, il semble basculer lorsqu'il change de direction quand le drapeau vert est cliqué :

```blocks3
when green flag clicked
point in direction (90)
set rotation style [gauche-droite v]
forever
move (5) steps
if on edge, bounce
```

Dans cet exemple, le bloc `s'orienter à`{:class="block3motion"} pointe automatiquement le sprite vers la droite (`90` degrés) lorsque le drapeau vert est cliqué. Si tu changes le nombre de degrés à `-90`, ton sprite pointera vers la gauche.

Ajoute un bloc `fixer le sens de rotation`{:class="block3motion"} et sélectionne `gauche-droite`{:class="block3motion"} dans le menu déroulant, afin que ton sprite ne se retrouve pas tête en bas lorsqu'il rebondit sur le bord de la scène.

**Astuce :** Tu peux faire glisser ton sprite sur la scène pour la déplacer vers la position y (haut-bas) souhaitée.

--- /collapse ---

--- collapse ---
---
title: Rebondir de haut en bas sur la Scène
---

--- no-print ---

**Fille qui saute** : [Voir à l'intérieur](https://scratch.mit.edu/projects/433595822/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433595822/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Ce code fait rebondir un sprite de haut en bas de la scène lorsque tu cliques sur le drapeau vert :

```blocks3
when green flag clicked
point in direction (0)
set rotation style [ne tourne pas v]
forever
move (5) steps
if on edge, bounce
```

Change le nombre de degrés du bloc `s'orienter à`{:class="block3motion"} à `0` pour faire pointer un sprite vers le haut.

Ajoute un bloc `fixer le sens de rotation`{:class="block3motion"} et sélectionne `ne tourne pas`{:class="block3motion"} dans le menu déroulant pour arrêter la rotation de ton sprite, même lorsqu'il rebondit.

**Astuce :** Tu peux faire glisser ton sprite sur la scène pour le déplacer vers la position x (gauche-droite) souhaitée.

--- /collapse ---

--- collapse ---
---
title: Rebondir de biais
---

--- no-print ---

**Ballon rebondissant** : [Voir à l'intérieur](https://scratch.mit.edu/projects/433536479/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433536479/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Ce code fait apparaître un sprite qui tourne de manière aléatoire lorsque l'on clique sur le drapeau vert :

```blocks3
when green flag clicked
point in direction (45)
set rotation style [à 360° v]
forever
move (5) steps
if on edge, bounce
```

Si ton sprite se déplace à `45` degrés, tu constateras qu'il semble rebondir sur le bord de la Scène sous un certain angle. Change le nombre de degrés du bloc `s'orienter à`{:class="block3motion"} à `45` pour faire rebondir ton sprite un peu partout.

Ajoute un bloc `fixer le sens rotation`{:class="block3motion"} et sélectionne `à 360°`{:class="block3motion"} dans le menu déroulant, de sorte que ton sprite tourne quand il rebondit sur le bord de la Scène.

--- /collapse ---

### Utiliser des coordonnées

Tu peux également `ajouter`{:class="block3motion"} et `mettre à`{:class="block3motion"} les coordonnées `x`{:class="block3motion"} et `y`{:class="block3motion"} et obtenir leurs valeurs pour les utiliser dans d'autres blocs :

[[[generic-scratch3-coordinates]]]

```blocks3 
change x by [10]

set x to [0]

change y by  [10]

set y to [0]

(x position)

(y position)
```

--- collapse ---
---
title: Je ne vois aucun bloc Mouvement
---

Si tu as sélectionné la Scène, tu ne verras aucun bloc `Mouvement`{:class="block3motion"}, car la scène ne peut pas bouger.

Clique sur un sprite dans le volet Sprite puis clique sur le volet **Code** pour voir les blocs `Mouvement`{:class="block3motion"}.

--- /collapse ---

