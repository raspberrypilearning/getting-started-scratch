## Capteurs

Les blocs de la catégorie `Capteurs`{:class="block3sensing"} sont utilisés pour obtenir la saisie de texte de vos utilisateurs, détecter les conditions et propager les valeurs de votre projet.

Il existe plusieurs blocs `Capteurs`{:class="block3sensing"} hexagonaux que tu peux imbriquer dans des blocs `Contrôle`{:class="block3control"} pour prendre des décisions et contrôler l'exécution des blocs.

Le bloc `touche`{:class="block3sensing"} a des options pour détecter si le sprite qui possède le script touche le pointeur de la souris (où tu as touché la dernière fois le doigt sur une tablette), le bord de la scène ou un autre sprite :

```blocks3
<touching (pointeur de souris v) ?>

<touching (bord v) ?>

<touching (Sprite2 v) ?>
```

Il existe des blocs pour détecter si le sprite qui possède le script touche une autre couleur (sur la scène ou un autre sprite), ou si une couleur sur ce sprite touche une autre couleur.

```blocks3
<touching color (#c5a97b) ?>

<color (#c219ed) is touching (#62d1e0) ?>
```

Le bloc `touche pressée ?`{:class="block3sensing"} a des options pour les touches numériques, alphabétiques et fléchées du clavier. Tu as besoin d'un clavier pour pouvoir saisir les touches. Il détecte si la touche est actuellement enfoncée :

```blocks3
<key (espace v) pressed?>
```

Le bloc `souris pressée ?`{:class="block3sensing"} détecte si la souris est actuellement enfoncée ou si l'écran est tapé ou touché dans le cas d'un écran tactile :

```blocks3
<mouse down?>
```

Les blocs `demander`{:class="block3sensing"} et `réponse`{:class="block3sensing"} sont utilisés pour obtenir la saisie de texte de l'utilisateur :

```blocks3
ask [Quel est ton nom] and wait

(answer) // le texte que l'utilisateur a tapé 
```

Le bloc `demander`{:class="block3sensing"} fonctionne avec un clavier ou avec un clavier virtuel sur l'écran d'une tablette.

Le bloc `réponse`{:class="block3sensing"} est un bloc qui rapporte une valeur et peut être utilisé comme variable.

[[[scratch3-ask-answer-chat]]]

La catégorie de blocs `Capteurs`{:class="block3sensing"} contient également plusieurs blocs qui peuvent être utilisés pour obtenir des valeurs :

```blocks3
(distance to (pointeur de souris v))

(distance to (Sprite2 v))
```

Tu peux détecter la position actuelle du pointeur de la souris (ou la position actuelle ou la plus récente de ton doigt sur une tablette) :

```blocks3
(mouse x)

(mouse y)
```

Tu peux détecter le `volume`{:class="block3sensing"} du son du microphone. Une fenêtre contextuelle demandera à l'utilisateur l'autorisation d'utiliser le microphone :

```blocks3
(loudness)
```

Le `chronomètre`{:class="block3sensing"} commence à compter lorsque le projet se charge, et peut être remis à `0` avec `réinitialiser le chronomètre`{:class="block3sensing"} :

```blocks3
(timer)

reset timer
```

Tu peux également accéder aux blocs d'obtention de valeurs de la Scène et d'autres sprites :

```blocks3
([backdrop # v] of (_stage_ v))

([x position v] of (Sprite2 v))

([costume # v] of (Sprite2 v))
```

Il existe des blocs d'obtention de valeurs liés à la date et à l'heure dans le monde réel, dans ton fuseau horaire local :

```blocks3
(current [year v]) // heure, minute, ...

(days since 2000)
```

