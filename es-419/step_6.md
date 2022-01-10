## Movimiento

Los bloques `Movimiento`{:class="block3motion"} te permiten mover tu objeto por el Escenario.

### Movement

El bloque `mover`{:class="block3motion"} es la forma más sencilla de empezar a mover un objeto:

```blocks3
move [10] steps
```

You can `go to`{:class="block3motion"} or `glide to`{:class="block3motion"} the mouse-pointer, a random position on the Stage (or your finger on a tablet), or another sprite:

```blocks3
go to (random position v)

glide [1] secs to (random position v)
```

You can also `go to`{:class="block3motion"} or `glide to`{:class="block3motion"} a position given by `x`{:class="block3motion"} and `y`{:class="block3motion"} coordinates on the Stage.

```blocks3
go to x: [0] y: [0] 

glide [1] secs to x: [0] y: [0]
```

[[[scratch3-glide-to-object]]]

**Consejo:** Cuando arrastras un objeto en el Escenario, los bloques de movimiento que usan las coordenadas `x`{:class="block3motion"} e `y`{:class="block3motion"} se actualizarán en el menú de bloques `Movimiento`{:class="block3motion"}. Las coordenadas `x`{:class="block3motion"} e `y`{:class="block3motion"} actuales se muestran en el panel Objetos.

### Rotación
También puedes cambiar la `dirección`{:class="block3motion"} a la que apunta un objeto. Esto cambia la dirección en la que se moverá el objeto si usas un bloque `mover`{:class="block3motion"}. It may also change the rotation of the sprite's costume depending on the `rotation-style`{:class="block3motion"} setting.

Cuando agregues un objeto, estará orientado hacia la derecha (90 grados). Puedes cambias ésto en el panel Objetos o usando bloques de código.

```blocks3
turn right [15] degrees

turn left [15] degrees

point in direction [90] // Click on 90 and drag the arrow to change

point towards (mouse-pointer v)

(direction)

set rotation style [left-right v] // or all-around or none
```

[[[scratch3-sprite-direction]]]

[[[scratch3-left-right-direction]]]

--- collapse ---
---
title: Spin around
---

--- no-print ---

**Spinning bat**: [See inside](https://scratch.mit.edu/projects/435704980/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435704980/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

This code makes a sprite spin when the green flag is clicked:

```blocks3
when flag clicked
forever
turn right (1) degrees :: motion
```

In a `turn`{:class="block3motion"} block within a `forever`{:class="block3control"} loop, change the number of degrees to `1` and your sprite will appear to spin.

**Consejo:** Si no agregas un bloque `mover`{:class="block3motion"}, tu objeto girará en la posición en la que se encuentra.

--- /collapse ---

--- collapse ---
---
title: Moverse en un círculo
---

--- no-print ---

**Moon orbit**: [See inside](https://scratch.mit.edu/projects/435701055/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435701055/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

This code makes a sprite fly in a circle when the green flag is clicked:

```blocks3
when green flag clicked
forever
move (1) steps
turn right (1) degrees :: motion
```

Change the values in a `move`{:class="block3motion"} block and `turn`{:class="block3motion"} block within a `forever`{:class="block3control"} loop to `1` and your sprite will appear to move in a big circle.

**Consejo:** Si quieres que tu objeto siempre comience en el centro del Escenario, puedes agregar un bloque `ir a x:`{:class="block3motion"}`0` `y:`{:class="block3motion"} `0` antes del bloque `por siempre`{:class="block3control"}.

--- /collapse ---

### Rebotar

El bloque `si toca un borde, rebotar`{:class="block3motion"} es realmente útil cuando quieres que un objeto rebote y permanezca en el Escenario:

```blocks3
if on edge, bounce
```

See some of the ways in which you can get your sprite to bounce around:

--- collapse ---
---
title: Rebotar por el Escenario
---

--- no-print ---

**Girl moving across the Stage**: [See inside](https://scratch.mit.edu/projects/433535326/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433535326/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Este código hace que un objeto rebote en los bordes izquierdo y derecho del Escenario. Because the sprite rotates horizontally, it appears to flip when it changes its direction when the green flag is clicked:

```blocks3
when green flag clicked
point in direction (90)
set rotation style [left-right v]
forever
move (5) steps
if on edge, bounce
```

En este ejemplo, el bloque `apuntar en dirección`{:class="block3motion"} apunta automáticamente al objeto hacia la derecha (`90` grados) al presionar la bandera verde. Si cambias el número de grados a `-90`, tu objeto apuntará hacia la izquierda.

Agrega un bloque `fijar estilo de rotación a`{:class="block3motion"} y selecciona `izquierda-derecha`{:class="block3motion"} en el menú desplegable, para que tu objeto no se dé la vuelta cuando rebote en el borde del Escenario.

**Consejo:** Puedes arrastrar tu objeto en el Escenario para moverlo a la posición y (arriba-abajo) que desees.

--- /collapse ---

--- collapse ---
---
title: Rebotar arriba y abajo por el Escenario
---

--- no-print ---

**Girl jumping**: [See inside](https://scratch.mit.edu/projects/433595822/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433595822/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Este código hace que un objeto rebote arriba y abajo por el escenario al presionar la bandera verde:

```blocks3
when green flag clicked
point in direction (0)
set rotation style [don't rotate v]
forever
move (5) steps
if on edge, bounce
```

Cambia el número de grados en el bloque `apuntar en dirección`{:class="block3motion"} a `0` para hacer que un objeto apunte hacia arriba.

Add a `set rotation style`{:class="block3motion"} block and select `don't rotate`{:class="block3motion"} in the drop-down menu to stop your sprite rotating, even when it bounces.

**Consejo:** Puedes arrastrar tu objeto por el Escenario para moverlo a la posición x (izquierda-derecha) que desees.

--- /collapse ---

--- collapse ---
---
title: Bounce at an angle
---

--- no-print ---

**Football bouncing**: [See inside](https://scratch.mit.edu/projects/433536479/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433536479/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Este código hace que un objeto parezca rotar aleatoriamente al presionar la bandera verde:

```blocks3
when green flag clicked
point in direction (45)
set rotation style [all around v]
forever
move (5) steps
if on edge, bounce
```

Si tu objeto se mueve a `45` grados, encontrarás que parece rebotar en el borde del escenario en un ángulo. Cambia el número de grados en el bloque `apuntar en dirección`{:class="block3motion"} a `45` para hacer que tu objeto rebote por todas partes.

Agrega un bloque `fijar estilo de rotación a`{:class="block3motion"} y selecciona `en todas las direcciones`{:class="block3motion"} en el menú desplegable, para que tu objeto gire cuando rebote en el borde del Escenario.

--- /collapse ---

### Usando coordenadas

También puedes `cambiar`{:class="block3motion"} y `fijar`{:class="block3motion"} las coordenadas `x`{:class="block3motion"} e `y`{:class="block3motion"} y obtener sus valores para usar en otros bloques:

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
title: No puedo ver ningún bloque de Movimiento
---

Si tienes el Escenario seleccionado no verás ningún bloque `Movimiento`{:class="block3motion"}, porque el Escenario no se puede mover.

Haz clic en un objeto en el panel de Objetos y luego haz clic en la pestaña **Código** para ver los bloques `Movimiento`{:class="block3motion"}.

--- /collapse ---

