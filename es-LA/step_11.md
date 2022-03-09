## Sensores

Los bloques en el menu de bloques `Sensores`{:class="block3sensing"} se utilizan para obtener la entrada de texto del usuario, detectar condiciones e informar sobre los valores en tu proyecto.

Hay varios bloques hexagonales `Sensores`{:class="block3sensing"} que puedes utilizar en bloques `Control`{:class="block3control"} para tomar decisiones y controlar cuándo se ejecutan los bloques.

El bloque `tocando`{:class="block3sensing"} tiene opciones para detectar si el objeto que posee el script está tocando el puntero del ratón (donde tocaste por última vez con el dedo en una tableta), el borde del Escenario u otro objeto:

```blocks3
<¿tocando (el puntero del ratón v)?>

<¿tocando (el borde v)?>

<¿tocando (Objeto2 v)?>
```

Hay bloques para detectar si el objeto que posee el script está tocando otro color (en el Escenario u otro objeto), o si un color en este objeto está tocando otro color.

```blocks3
<touching color (#c5a97b) ?>

<color (#c219ed) is touching (#62d1e0) ?>
```

El bloque `tecla presionada`{:class="block3sensing"} tiene opciones para teclas numéricas, letras y flechas. Necesitas un teclado para poder ingresar teclas. Detecta si la tecla está siendo presionada en ese momento:

```blocks3
<key (space v) pressed?>
```

El bloque `¿ratón presionado?`{:class="block3sensing"} detecta si el ratón está siendo presionado, o si la pantalla está siendo pulsada o tocada en una pantalla táctil:

```blocks3
<mouse down?>
```

Los bloques `preguntar`{:class="block3sensing"} y `respuesta`{:class="block3sensing"} se utilizan para obtener la entrada de texto del usuario:

```blocks3
ask [Cómo te llamas] and wait

(answer) // el texto que el usuario escribió 
```

El bloque `preguntar`{:class="block3sensing"} funciona con un teclado o con un teclado virtual en pantalla en una tableta.

El bloque `respuesta`{:class="block3sensing"} es un bloque informador que informa de un valor y se puede utilizar como variable.

[[[scratch3-ask-answer-chat]]]

El menú de bloques `Sensores`{:class="block3sensing"} también contiene varios bloques informadores que se pueden utilizar para obtener valores:

```blocks3
(distance to (mouse-pointer v))

(distance to (Sprite2 v))
```

Puedes detectar la posición actual del puntero del mouse (o la posición actual o más reciente de tu dedo en una tableta):

```blocks3
(mouse x)

(mouse y)
```

Puedes detectar el `volumen`{:class="block3sensing"} del sonido del micrófono. Una ventana emergente le pedirá al usuario permiso para usar el micrófono:

```blocks3
(loudness)
```

El `cronómetro`{:class="block3sensing"} comienza a contar cuando se carga el proyecto y se puede volver a establecer en `0` con `reiniciar cronómetro`{:class="block3sensing"}:

```blocks3
(timer)

reset timer
```

También puedes acceder a los informadores para el Escenario y otros objetos:

```blocks3
([backdrop # v] of (_stage_ v))

([x position v] of (Sprite2 v))

([costume # v] of (Sprite2 v))
```

Hay informadores relacionados con la fecha y la hora en el mundo real, en tu zona horaria local:

```blocks3
(current [year v]) // hora, minuto, ...

(days since 2000)
```

