## Eventos

Los bloques en el menú `Eventos`{:class="block3events"} controlan cuando se inician los scripts.

**Bloques de sombrero** ejecutan los bloques debajo de ellos cuando ocurre un evento en particular. Están redondeados en la parte superior, como un sombrero, por lo que ningún bloque puede estar por encima de ellos.

Puedes usar:

```blocks3

when flag clicked // ejecuta bloques al presionar la fecha verde que está sobre el Escenario

when this sprite clicked // ejecuta bloques al hacer clic en el objeto de este script

when stage clicked // ejecuta los bloques cuando se hace clic en el escenario

```

**Consejo:** El bloque `cuando se hace clic en el escenario`{:class="block3events"} solo está disponible cuando se trabaja en el área de Código del escenario.

Si estás usando una computadora con un teclado, puedes utilizar `al presionar tecla`{:class="block3events"}:

```blocks3
when [space v] key pressed // cambiar a teclas de número, letra o flecha
```

También puedes usar un bloque `cuando el fondo cambia a`{:class="block3events"} para iniciar una secuencia de comandos cuando cambia el fondo.

[[[scratch3-changing-backdrops-pages-levels]]]

[[[scratch3-show-hide-sprites-backdrops]]]


El bloque `when >`{:class="block3events"} tiene dos versiones:

```blocks3
when [loudness v] > (10) // ejecuta bloques cuando el micrófono detecta sonido

when [timer v] > (10) // ejecuta bloques cuando el cronómetro llega a 10 segundos
```

[[[scratch3-time-delay]]]


Los dos últimos bloques del menú `Eventos`{:class="block3events"} son bloques `enviar`{:class="block3events"}. Puedes usar `al recibir (mensaje v)`{:class="block3events"} para iniciar un script cuando cualquier objeto ejecute un bloque igual `enviar (mensaje v)`{:class="block3events"}.

[[[generic-scratch3-broadcast-message]]]

