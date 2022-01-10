## Control

`Control`{:class="block3control"} blocks control the order that blocks run in, including decisions (selection) and loops (repetition).


El bloque `esperar`{:class="block3control"} se demora unos segundos antes de ejecutar el siguiente bloque.

```blocks3
wait (1) seconds// delay for 1 second

wait (0.1) seconds// delay for one tenth of a second
```

Loops control how many time the code inside them runs.

```blocks3
repeat (4) // run the blocks inside four time

end
```

```blocks3
forever // run the blocks inside until stopped

end
```

[[[scratch3-forever-condition]]]

**Consejo:** Puedes detener un bloque `por siempre`{:class="block3events"} pulsando el botón Detener sobre el Escenario, o usando los bloques `detener`{:class="block3control"}.

Hay tres opciones para el bloque `detener`{:class="block3events"}:

```blocks3
stop [all v] // stop all scripts in all sprites

stop [this script v]

stop [other scripts in sprite v]
```

The `if...then`{:class="block3control"} and `if...then...else`{:class="block3control"} blocks are used to make decisions about which code blocks to run next. A esto a veces se le llama **selección**. El bloque `si...entonces`{:class="block3control"} verifica una **condición** con forma hexagonal y ejecuta los bloques de código en el interior, si la condición es **verdadera**. El bloque `si...entonces...si no`{:class="block3control"} tiene una sección adicional para ejecutar los bloques de código en su interior, si la condición es **falsa**.

```blocks3
if <> then

end

if <> then

else

end
```

[[[scratch3-if-then-else]]]

Puedes encontrar bloques de forma hexagonal para usar como condiciones en los menús de los bloques `Operadores`{:class="block3operators"} y `Sensores`{:class="block3sensing"}.

Los bloques `esperar hasta que`{:class="block3control"} y el `repetir hasta que`{:class="block3control"} también usan condiciones:

```blocks3
wait until <> // delay until the condition is true


repeat until <> // repeat the blocks inside until the condtion is true

end
```

Un **clon** es una copia de un objeto, tiene los disfraces, scripts y sonidos del objeto del que se clonó en el momento de la clonación. Hay una serie de bloques que se pueden usar para clonar objetos.

With the `create clone of [myself v]`{:class="block3control"} block, a sprite can create a clone of itself or of another sprite in the project.

```blocks3
create clone of [myself v] // clones the sprite that runs this block


create clone of [Butterfly 1 v] // clones another sprite in the project
```

El bloque de sombrero `al comenzar como clon`{:class="block3control"} se usa para activar un nuevo script una vez que se ha creado el clon. The clone will exist in the project until the `delete this clone`{:class="block3control"} cap block is used.

Using the `when I start as a clone`{:class="block3control"} hat block then including the `create clone of [myself v]`{:class="block3control"} block in the script underneath means it is also possible for clones to create other clones.

```blocks3
when I start as a clone // the script that runs when the clone is created


delete this clone // stops the clone's scripts and deletes it
```

There is a maximum number of clones a sprite can have at any point, at the time of writing this is `300`.

--- collapse ---
---
title: Clones de clones
---

**Clones**: [See inside](https://scratch.mit.edu/projects/567544298/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567544298/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /collapse ---

