## Sensores

Os blocos no menu `Sensores`{:class="block3sensing"} são usados para obter textos do usuário, detectar condições e relatar valores em seu projeto.

Existem vários blocos hexagonais na categoria `Sensores`{:class="block3sensing"} que você pode usar em blocos da categoria `Controle`{:class="block3control"} para tomar decisões e controlar quando os blocos são executados.

O bloco `tocando em`{:class="block3sensing"} tem opções para detectar se o ator que possui seu próprio script está tocando o ponteiro do mouse (onde seu dedo tocou por último na tela do tablet), na borda do Palco, ou um outro ator:

```blocks3
<touching (mouse-pointer v) ?>

<touching (edge v) ?>

<touching (Sprite2 v) ?>
```

Existem blocos para detectar se o ator que possui seu próprio script está tocando em outra cor (no Palco ou em outro ator), ou se uma cor neste ator está tocando em outra cor.

```blocks3
<touching color (#c5a97b) ?>

<color (#c219ed) is touching (#62d1e0) ?>
```

A bloco `tecla pressionada`bloco{:class="block3sensing"} tem opções para números, letras e setas de direção. Você precisa de um teclado para pressionar as teclas. Ele detecta se uma tecla está sendo pressionada:

```blocks3
<key (space v) pressed?>
```

The `mouse down`{:class="block3sensing"} block detects whether the mouse is currently pressed, or the screen is being tapped or touched on a touchscreen:

```blocks3
<mouse down?>
```

The `ask`{:class="block3sensing"} and `answer`{:class="block3sensing"} blocks are used to get text input from the user:

```blocks3
ask [What's your name] and wait

(answer) // the text the the user typed 
```

The `ask`{:class="block3sensing"} block works with a keyboard or with a virtual on-screen keyboard on a tablet.

The `answer`{:class="block3sensing"} block is a reporter block that reports a value and can be used as a variable.

[[[scratch3-ask-answer-chat]]]

The `Sensing`{:class="block3sensing"} blocks menu also contains several reporter blocks that can be used to get values:

```blocks3
(distance to (mouse-pointer v))

(distance to (Sprite2 v))
```

You can detect the current position of the mouse-pointer (or the current or most recent position of your finger on a tablet):

```blocks3
(mouse x)

(mouse y)
```

You can detect the `loudness`{:class="block3sensing"} of sound from the microphone. A pop-up window will ask the user for permission to use the microphone:

```blocks3
(loudness)
```

The `timer`{:class="block3sensing"} starts counting when the project loads, and can be set back to `0` with `reset timer`{:class="block3sensing"}:

```blocks3
(timer)

reset timer
```

You can also access reporters for the Stage and other sprites:

```blocks3
([backdrop # v] of (_stage_ v))

([x position v] of (Sprite2 v))

([costume # v] of (Sprite2 v))
```

There are reporters related to the date and time in the real world, in your local timezone:

```blocks3
(current [year v]) // hour, minute, ...

(days since 2000)
```

