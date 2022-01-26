## Eventos

Los bloques en el menú `Eventos`{:class="block3events"} controlan cuando se inician los scripts.

**Bloques de sombrero** ejecutan los bloques debajo de ellos cuando ocurre un evento en particular. Están redondeados en la parte superior, como un sombrero, por lo que ningún bloque puede estar por encima de ellos.

Puedes usar:

```blocks3

when flag clicked // run blocks when the green flag above the Stage is clicked

when this sprite clicked // run the blocks when the sprite for this script is clicked

when stage clicked // run the blocks when the stage is clicked

```

**Consejo:** El bloque `cuando se hace clic en el escenario`{:class="block3events"} solo está disponible cuando se trabaja en el área de Código del escenario.

Si estás usando una computadora con un teclado, puedes utilizar `al presionar tecla`{:class="block3events"}:

```blocks3
when [space v] key pressed // change to number, letter or arrow keys
```

También puedes usar un bloque `cuando el fondo cambia a` {:class="block3events"} para iniciar una secuencia de comandos cuando cambia el fondo.

[[[scratch3-changing-backdrops-pages-levels]]]

[[[scratch3-show-hide-sprites-backdrops]]]


El bloque `when >`{:class="block3events"} tiene dos versiones:

```blocks3
when [loudness v] > (10) // run blocks when the microphone detects sound

when [timer v] > (10) // run blocks when the timer reaches 10 seconds
```

[[[scratch3-time-delay]]]


Los dos últimos bloques del menú `Eventos`{:class="block3events"} son bloques `enviar`{:class="block3events"}. Puedes usar `al recibir (mensaje v)`{:class="block3events"} para iniciar un script cuando cualquier objeto ejecute un bloque igual `enviar (mensaje v)`{:class="block3events"}.

[[[generic-scratch3-broadcast-message]]]

