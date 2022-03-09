## Movimiento

Los bloques `Movimiento`{:class="block3motion"} te permiten mover tu objeto por el Escenario.

### Mover

El bloque `mover`{:class="block3motion"} es la forma más sencilla de empezar a mover un objeto:

```blocks3
move [10] steps
```

Puedes `ir a`{:class="block3motion"} o `desplazar en`{:class="block3motion"} puntero del ratón, posición aleatoria en el Escenario (o tu dedo en una tableta), u otro objeto:

```blocks3
go to (random position v)

glide [1] secs to (random position v)
```

También puedes `ir a`{:class="block3motion"} o `desplazar en`{:class="block3motion"} una posición dada por las coordenadas `x`{:class="block3motion"} e `y`{:class="block3motion"} en el Escenario.

```blocks3
go to x: [0] y: [0] 

glide [1] secs to x: [0] y: [0]
```

[[[scratch3-glide-to-object]]]

**Consejo:** Cuando arrastras un objeto en el Escenario, los bloques de movimiento que usan las coordenadas `x`{:class="block3motion"} e `y`{:class="block3motion"} se actualizarán en el menú de bloques `Movimiento`{:class="block3motion"}. Las coordenadas `x`{:class="block3motion"} e `y`{:class="block3motion"} actuales se muestran en el panel Objetos.

### Rotación
También puedes cambiar la `dirección`{:class="block3motion"} a la que apunta un objeto. Esto cambia la dirección en la que se moverá el objeto si usas un bloque `mover`{:class="block3motion"}. También puede cambiar la rotación del disfraz del objeto dependiendo de la configuración del `estilo de rotación`{:class="block3motion"}.

Cuando agregues un objeto, estará orientado hacia la derecha (90 grados). Puedes cambias ésto en el panel Objetos o usando bloques de código.

```blocks3
turn right [15] degrees

turn left [15] degrees

point in direction [90] // Haz clic en 90 y arrastra la flecha para cambiar

point towards (mouse-pointer v)

(direction)

set rotation style [left-right v] // o en todas las direcciones o no rotar
```

[[[scratch3-sprite-direction]]]

[[[scratch3-left-right-direction]]]

--- collapse ---
---
title: Girar
---

--- no-print ---

**Murciélago giratorio**: [Ver dentro](https://scratch.mit.edu/projects/435704980/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435704980/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Este código hace girar un objeto al presionar la bandera verde:

```blocks3
when flag clicked
forever
turn right (1) degrees :: motion
```

En un bloque `girar`{:class="block3motion"} dentro de un bucle `por siempre`{:class="block3control"}, cambia el número de grados a `1` y tu objeto parecerá girar.

**Consejo:** Si no agregas un bloque `mover`{:class="block3motion"}, tu objeto girará en la posición en la que se encuentra.

--- /collapse ---

--- collapse ---
---
title: Moverse en un círculo
---

--- no-print ---

**Órbita Lunar**: [Ver dentro](https://scratch.mit.edu/projects/435701055/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435701055/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Este código hace volar un objeto en círculo cuando al presionar la bandera verde:

```blocks3
when green flag clicked
forever
move (1) steps
turn right (1) degrees :: motion
```

Cambia los valores en un bloque `mover`{:class="block3motion"} y bloque `girar`{:class="block3motion"} dentro de un bucle `por siempre`{:class="block3control"} a `1` y tu objeto parecerá moverse en un gran círculo.

**Consejo:** Si quieres que tu objeto siempre comience en el centro del Escenario, puedes agregar un bloque `ir a x:`{:class="block3motion"}`0` `y:`{:class="block3motion"} `0` antes del bloque `por siempre`{:class="block3control"}.

--- /collapse --- 

### Rebotar

El bloque `si toca un borde, rebotar`{:class="block3motion"} es realmente útil cuando quieres que un objeto rebote y permanezca en el Escenario:

```blocks3
if on edge, bounce
```

Mira algunas de las formas en las que puedes hacer que tu objeto rebote:

--- collapse ---
---
title: Rebotar por el Escenario
---

--- no-print ---

**Muchacha moviéndose por el Escenario**: [Ver dentro](https://scratch.mit.edu/projects/433535326/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433535326/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Este código hace que un objeto rebote en los bordes izquierdo y derecho del Escenario. Debido a que el objeto gira horizontalmente, parece que se voltea cuando cambia de dirección al presionar la bandera verde:

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

**Muchacha saltando**: [Ver dentro](https://scratch.mit.edu/projects/433595822/editor){:target="_blank"}

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

Agrega un bloque `fijar estilo de rotación a`{:class="block3motion"} y selecciona `no rotar`{:class="block3motion"} en el menú desplegable para detener la rotación de tu objeto, incluso cuando rebote.

**Consejo:** Puedes arrastrar tu objeto por el Escenario para moverlo a la posición x (izquierda-derecha) que desees.

--- /collapse ---

--- collapse ---
---
title: Rebotar en un ángulo
---

--- no-print ---

**Pelota de fútbol rebotando**: [Ver dentro](https://scratch.mit.edu/projects/433536479/editor){:target="_blank"}

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

