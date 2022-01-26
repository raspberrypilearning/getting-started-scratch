## Control

Los bloques `Control`{:class="block3control"} controlan el orden en que se ejecutan los bloques, incluidas las decisiones (selección) y los bucles (repetición).


El bloque `esperar`{:class="block3control"} se demora unos segundos antes de ejecutar el siguiente bloque.

```blocks3
wait (1) seconds// delay for 1 second

wait (0.1) seconds// delay for one tenth of a second
```

Los bucles controlan cuántas veces se ejecuta el código dentro de ellos.

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

Los bloques `si...entonces`{:class="block3control"} y `si...entonces...si no`{:class="block3control"} se utilizan para tomar decisiones sobre qué bloques de código ejecutar a continuación. A esto a veces se le llama **selección**. El bloque `si...entonces`{:class="block3control"} verifica una **condición** con forma hexagonal y ejecuta los bloques de código en el interior, si la condición es **verdadera**. El bloque `si...entonces...si no`{:class="block3control"} tiene una sección adicional para ejecutar los bloques de código en su interior, si la condición es **falsa**.

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

Con el bloque `crear clon de [mí mismo]`{:class="block3control"}, un objeto puede crear un clon de sí mismo o de otro objeto en el proyecto.

```blocks3
create clone of [myself v] // clones the sprite that runs this block


create clone of [Butterfly 1 v] // clones another sprite in the project
```

El bloque de sombrero `al comenzar como clon`{:class="block3control"} se usa para activar un nuevo script una vez que se ha creado el clon. El clon existirá en el proyecto hasta que se use el bloque de sombrero `eliminar este clon`{:class="block3control"}.

Usando el bloque de sombrero `al comenzar como clon`{:class="block3control"} y luego incluyendo el bloque `crear clon de [mí mismo]`{:class="block3control"} en el script debajo significa que también es posible que los clones creen otros clones.

```blocks3
when I start as a clone // the script that runs when the clone is created


delete this clone // stops the clone's scripts and deletes it
```

Hay un número máximo de clones que un objeto puede tener, al momento en el que esto fue escrito es `300`.

--- collapse ---
---
title: Clones de clones
---

**Clones**: [Ver dentro](https://scratch.mit.edu/projects/567544298/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567544298/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /collapse ---

