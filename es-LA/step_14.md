## Mis bloques

`Mis bloques`{:class="block3myblocks"} te permite crear nuevos bloques para un objeto. Le das un nombre al bloque y luego tienes que `definir`{:class="block3myblocks"} lo que hace el nuevo bloque usando otros bloques Scratch. Puedes usar tu nuevo bloque en cualquier script del objeto al que pertenece el bloque.

Este ejemplo define un bloque `hablar`{:class="block3myblocks"} que hace que un objeto cambie de disfraz:

**Pingüino chirría**: [Ver dentro](https://scratch.mit.edu/projects/567554899/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567554899/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

```blocks3
define palabras
switch costume to (penguin2-b v)
repeat (2)
play sound (chirp v) until done
end
switch costume to (penguin2-a v)

when this sprite clicked
palabras

when [space v] key pressed
palabras
```

Puedes utilizar `Mis Bloques`{:class="block3myblocks"} para **organizar** tu código. Es más sencillo agrupar todos los bloques que hacen que un objeto hable y luego usar un bloque `hablar`{:class="block3myblocks"} cuando quieras que tu objeto hable.

Si decides que quieres cambiar la forma en que habla tu objeto entonces sólo tienes que cambiar el código en un lugar.

### Mis bloques con entradas

También puedes agregar **entradas** a `Mis bloques`{:class="block3myblocks"} para que utilicen los valores que tú proporciones cuando uses el bloque.

**Pingüino habla**: [Ver dentro](https://scratch.mit.edu/projects/567538874/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567538874/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

```blocks3
define palabras (palabras)
switch costume to (penguin2-b v)
say (palabras) // utiliza la entrada proporcionada
repeat (2)
play sound (chirp v) until done
end
say (palabras)
switch costume to (penguin2-a v)

when this sprite clicked
palabras [hola]

when [space v] key pressed
palabras [hola]
```

[[[generic-scratch3-make-block]]]

--- collapse ---
---
title: Usar Mis Bloques para organizar el código
---
La forma más sencilla de utilizar `Mis Bloques`{:class="block3myblocks"} es para ayudar a organizar tu código. Aquí tienes un ejemplo sencillo.

```blocks3
define mover a la derecha
if <not <touching (edge v) ?>> then
switch costume to [derecha_1 v]
change x by (2)
switch costume to [derecha_2 v]
change x by (2)
switch costume to [derecha_3 v]
change x by (2)
end

define mover a la izquierda
if <not <touching (edge v) ?>> then
switch costume to [izquierda_1 v]
change x by (-2)
switch costume to [izquierda_2 v]
change x by (-2)
switch costume to [izquierda_3 v]
change x by (-2)
end

when flag clicked
forever
if <key (right arrow v) pressed> then
mover a la derecha
end
if <key (left arrow v) pressed> then
mover a la izquierda
```

--- /collapse ---

`Mis bloques`{:class="block3myblocks"} son similares a 'procedimientos', 'funciones' o 'métodos' en otros lenguajes de programación.
