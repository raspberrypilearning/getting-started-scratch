## Mes blocs

`Mes blocs`{:class="block3myblocks"} te permet de créer de nouveaux blocs pour un sprite. Tu donnes un nom au bloc, puis tu peux `définir`{:class="block3myblocks"} ce que le nouveau bloc fait en utilisant d'autres blocs Scratch. Tu peux utiliser ton nouveau bloc dans n'importe quel script sur le sprite qui possède le bloc.

Cet exemple définit un bloc `parler`{:class="block3myblocks"} qui change le costume d'un sprite :

**Pingouin pépie** : [Voir à l'intérieur](https://scratch.mit.edu/projects/567554899/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567554899/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

```blocks3
define talk
switch costume to (penguin2-b v)
repeat (2)
play sound (chirp v) until done
end
switch costume to (penguin2-a v)

when this sprite clicked
talk

when [space v] key pressed
talk
```

Tu peux utiliser `Mes blocs`{:class="block3myblocks"} pour **organiser** ton code. Il est plus simple de regrouper tous les blocs qui font parler un sprite, puis d'utiliser un seul bloc `parler`{:class="block3myblocks"} lorsque tu veux que ton sprite parle.

Si tu décides que tu veux changer la façon dont ton sprite parle, tu n'as qu'à changer le code à un seul endroit.

### Mes blocs avec paramètres entrants

Tu peux également ajouter des **paramètres entrants** à `Mes blocs`{:class="block3myblocks"} afin qu'ils utilisent les valeurs que tu fournis lorsque tu utilises le bloc.

**Pingouin parle** : [Voir à l'intérieur](https://scratch.mit.edu/projects/567538874/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567538874/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

```blocks3
define talk (words)
switch costume to (penguin2-b v)
say (words) // use the provided input
repeat (2)
play sound (chirp v) until done
end
say (words)
switch costume to (penguin2-a v)

when this sprite clicked
talk [hello]

when [space v] key pressed
talk [hi]
```

[[[generic-scratch3-make-block]]]

--- collapse ---
---
title: Utiliser Mes blocs pour organiser le code
---
La façon la plus simple d'utiliser `Mes Blocs`{:class="block3myblocks"} est d'aider à organiser ton code. Voici un exemple simple.

```blocks3
define move right
if <not <touching (edge v) ?>> then
switch costume to [right_1 v]
change x by (2)
switch costume to [right_2 v]
change x by (2)
switch costume to [right_3 v]
change x by (2)
end

define move left
if <not <touching (edge v) ?>> then
switch costume to [left_1 v]
change x by (-2)
switch costume to [left_2 v]
change x by (-2)
switch costume to [left_3 v]
change x by (-2)
end

when flag clicked
forever
if <key (right arrow v) pressed> then
move right
end
if <key (left arrow v) pressed> then
move left
```

--- /collapse ---

`Mes blocs`{:class="block3myblocks"} sont similaires aux 'procédures', 'fonctions' ou 'méthodes' dans d'autres langages de programmation.
