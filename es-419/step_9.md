## Eventos

Blocks in the `Events`{:class="block3events"} menu control when scripts are started.

**Bloques de sombrero** ejecutan los bloques debajo de ellos cuando ocurre un evento en particular. Están redondeados en la parte superior, como un sombrero, por lo que ningún bloque puede estar por encima de ellos.

Puedes usar:

```blocks3

when flag clicked // run blocks when the green flag above the Stage is clicked

when this sprite clicked // run the blocks when the sprite for this script is clicked

when stage clicked // run the blocks when the stage is clicked

```

**Consejo:** El bloque `cuando se hace clic en el escenario`{:class="block3events"} solo está disponible cuando se trabaja en el área de Código del escenario.

If you are on a computer with a keyboard, you can use `when key pressed`{:class="block3events"}:

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


The last two blocks in the `Events`{:class="block3events"} menu are `broadcast`{:class="block3events"} blocks. You can use `when i receive (message v)`{:class="block3events"} to start a script when any sprite runs a matching `broadcast (message v)`{:class="block3events"} block.

[[[generic-scratch3-broadcast-message]]]

