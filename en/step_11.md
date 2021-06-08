## Sensing

The blocks in the `Sensing`{:class="block3sensing"} blocks menu are used to get user text input, detect conditions, and report on values in your project.

There are several hexagonal `Sensing`{:class="block3sensing"} blocks that you can use in `Control`{:class="block3control"} blocks to make decisions and control when blocks run.

The `touching`{:class="block3sensing"} block has options for detecting whether the sprite that owns the script is touching the mouse pointer (where you finger last touched on a tablet), the edge of the Stage or another sprite:

```blocks
<touching (mouse-pointer v) ?>

<touching (edge v) ?>

<touching (Sprite2 v) ?>
```

There are blocks for detecting whether the sprite that owns the script is touching another colour (on the Stage or another sprite), or whether a colour on this sprite is touching another colour.

```blocks3
<touching color (#c5a97b) ?>

<color (#c219ed) is touching (#62d1e0) ?>
```

The `key pressed`{:class="block3sensing"} block has options for number, letter and arrow keys. You need a keyboard to be able to enter keys. It detects whether the key is currently being pressed:

```blocks
<key (space v) pressed?>
```

The `mouse down`{:class="block3sensing"} block detects whether the mouse is currently pressed, or the screen is being tapped or touched on a touchscreen:

```blocks
<mouse down?>
```

The `ask`{:class="block3sensing"} and `answer`{:class="block3sensing"} blocks are used to get text input from the user:

Answer is a 'reporter' that you can use as a variable.

```blocks
ask [What's your name] and wait

(answer) // the text the the user typed 
```

The `ask`{:class="block3sensing"} block works with a keyboard or with a virtual on-screen keyboard on a tablet.

[[[scratch3-ask-answer-chat]]]

The `Sensing`{:class="block3sensing"} blocks menu also contains several 'reporter' blocks that can be used to get values:

```blocks3
(distance to (mouse-pointer v))

(distance to (Sprite2 v))
```

You can detect the current position of the mouse pointer (or the current or most recent position of your finger on a tablet): 

```blocks3
(mouse x)

(mouse y)
```

You can detect the `loudness`{:class="block3sensing"} of sound from the microphone, a pop-up will ask the user for permission to use the microphone:

```blocks3
(loudness)
```

The `timer`{:class="block3sensing"} starts counting when the project loads and can be set back to `0` with `reset timer`{:class="block3sensing"}:

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

