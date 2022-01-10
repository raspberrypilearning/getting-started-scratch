## Contrôle

Les blocs `Contrôle`{:class="block3control"} contrôlent l'ordre dans lequel les blocs s'exécutent, y compris les décisions (sélection) et les boucles (répétition).


Le bloc `attendre`{:class="block3control"} attend un certain nombre de secondes avant d'exécuter le bloc suivant.

```blocks3
wait (1) seconds// delay for 1 second

wait (0.1) seconds// delay for one tenth of a second
```

Les boucles contrôlent le nombre d'exécutions du code qu'elles contiennent.

```blocks3
repeat (4) // run the blocks inside four time

end
```

```blocks3
forever // run the blocks inside until stopped

end
```

[[[scratch3-forever-condition]]]

**Astuce :** Tu peux arrêter un `répéter indéfiniment`{:class="block3events"} en cliquant sur le bouton Stop au-dessus de la Scène, ou en utilisant les blocs `stop`{:class="block3control"}.

Il existe trois options pour le bloc `stop`{:class="block3events"} :

```blocks3
stop [all v] // stop all scripts in all sprites

stop [this script v]

stop [other scripts in sprite v]
```

Les blocs `si...alors`{:class="block3control"} et `si...alors...sinon`{:class="block3control"} sont utilisés pour prendre des décisions sur les blocs de code à exécuter ensuite. Ceci est parfois appelé **sélection**. Le bloc `si...alors`{:class="block3control"} vérifie une **condition** en forme d'hexagone et exécute les blocs de code à l'intérieur, si la condition est **vraie**. Le bloc `si...alors...sinon`{:class="block3control"} a une section supplémentaire pour exécuter les blocs de code à l'intérieur, si la condition est **fausse**.

```blocks3
if <> then

end

if <> then

else

end
```

[[[scratch3-if-then-else]]]

Vous pouvez trouver des blocs de forme hexagonale à utiliser comme conditions dans les catégories `Opérateurs`{:class="block3operators"} et `Capteurs`{:class="block3sensing"}.

Les blocs `attendre jusqu'à ce que`{:class="block3control"} et `répéter jusqu'à ce que`{:class="block3control"} utilisent également des conditions :

```blocks3
wait until <> // delay until the condition is true


repeat until <> // repeat the blocks inside until the condtion is true

end
```

Un **clone** est une copie d'un sprite, il a les costumes, les scripts et les sons détenus par le sprite à partir duquel il a été cloné au moment du clonage. Il existe un certain nombre de blocs qui peuvent être utilisés pour cloner des sprites.

Avec le bloc `créer un clone de [moi-même v]`{:class="block3control"}, un sprite peut créer un clone de lui-même ou d'un autre sprite dans le projet.

```blocks3
create clone of [myself v] // clones the sprite that runs this block


create clone of [Butterfly 1 v] // clones another sprite in the project
```

Le bloc événement `quand je commence comme un clone`{:class="block3control"} est utilisé pour déclencher un nouveau script une fois le clone créé. Le clone existera dans le projet jusqu'à ce que le `supprimer ce clone`{:class="block3control"} soit utilisé.

Utiliser le `quand je commence comme un clone`{:class="block3control"} puis inclure le bloc `créer un clone de [moi-même v]`{:class="block3control"} dans le script en dessous signifie qu'il est également possible que les clones créent d'autres clones.

```blocks3
when I start as a clone // the script that runs when the clone is created


delete this clone // stops the clone's scripts and deletes it
```

Il y a un nombre maximum de clones qu'un sprite peut avoir à tout moment, au moment de la rédaction de ce manuel, c'est `300`.

--- collapse ---
---
title : Clones de clones
---

**Clones** : [Voir à l'intérieur](https://scratch.mit.edu/projects/567544298/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567544298/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /collapse ---

