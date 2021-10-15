## Looks

`Looks`{:class="block3looks"} blocks control a sprite's appearance on the Stage.

Sprites can communicate using `Looks`{:class="block3looks"}, through a `say`{:class="block3looks"} speech bubble, a `think`{:class="block3looks"} thought bubble, or through their `graphic effects`{:class="block3looks"}.

### Say and think

```blocks3
say () for () seconds

say ()

think () for () seconds

think ()
```

--- collapse ---
---
title: Use a speech bubble to communicate
---

Sprites can `say`{:class="block3looks"} and `think`{:class="block3looks"} to communicate.

The `say () for () seconds`{:class="block3looks"} and `think () for () seconds`{:class="block3looks"} blocks are used to say or think something for a set amount of time.

```blocks3
when this sprite clicked
say [Hello!] for [2] seconds // hide speech after 2 seconds
```

The sprite will show a speech bubble for two seconds when clicked.

**Space talk**: [See inside](https://scratch.mit.edu/projects/485673032/editor){:target="_blank"}

Click on the sprites to see them communicate with speech and thought.

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/485673032/?autostart=false" frameborder="0"></iframe>
</div>

The `say ()`{:class="block3looks"} and `think ()`{:class="block3looks"} blocks are used to say or think something, until another message or an empty `say ()`{:class="block3looks"} or `think ()`{:class="block3looks"} block replaces it.

--- /collapse ---

### Size

Set or change the `size`{:class="block3looks"} of your sprites.

```blocks3
change size by ()

set size to () %

(size)
```

--- collapse ---
---
title: Set the size of your sprite
---

When you add a sprite to your project, its size is set to `100` percent. This may be too big or too small for your project.

You can use code to set the size of a sprite. To do this, use a `set size to`{:class="block3looks"} block:

```blocks3
set size to (50) %
```

If you set the size of a sprite to `50` percent, it will be half as tall and half as wide. If you set the size of a sprite to `200` percent, it will be twice as tall and twice as wide.

To set the size of a sprite when the project is started, place a `set size to`{:class="block3looks"} block under a `when green flag clicked`{:class="block3events"} block:

```blocks3
when green flag clicked
set size to (50) %
```

You can also quickly set the size of a sprite in the **Size** property in the Sprite pane below the Stage:

![The Size box highlighted in the Sprite pane.](images/spriteSize.png){:width="400px"}

--- /collapse ---

### Graphic effects

Set or change a range of visual effects, such as colour, fisheye, whirl, pixelate, mosaic, brightness and ghost.

```blocks3
change [color v] effect by ()

set [color v] effect to ()

clear graphic effects
```

[[[scratch3-graphic-effects]]]

### Costumes

To create an animation effect with your sprites, you can change their costumes.

```blocks3
switch costume to ( v)

next costume

(costume [number v])
```

[[[scratch3-change-costumes-to-show-mood]]]

--- collapse ---
---
title: Change looks to create an animation effect
---

**Beating heart**: [See inside](https://scratch.mit.edu/projects/435725413/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/435725413/?autostart=false" frameborder="0"></iframe>
</div>

You can use the `set size to`{:class="block3looks"} or `change size by`{:class="block3looks"} blocks to create a pulsing effect, such as a beating heart.

**Note:** The `set size to`{:class="block3looks"} block sets the size to a specific value, while the `change size by`{:class="block3looks"} block changes the value from what it was before, e.g. `change size by`{:class="block3looks"} `10` adds 10 to the value of the size.

```blocks3
when green flag clicked
set size to (160) %
forever
change size by (40)
wait (0.2) seconds
change size by (20)
wait (0.2) seconds
change size by (-20)
wait (0.2) seconds
change size by (-40)
wait (0.2) seconds
end
```

This code uses a series of `change size by`{:class="block3looks"} and `wait`{:class="block3control"} blocks to make the heart grow and shrink. Try to create your own pulsing sprite.

You could also use the `change graphic effect by`{:class="block3looks"} block to create a sprite that continues to change its appearance.

```blocks3
when green flag clicked
change [ghost v] effect by (75)
wait (1) seconds
change [ghost v] effect by (-75)
```

**Note:** If you use code that changes a graphic effect and then changes it back again, remember to use a `wait`{:class="block3control"} block in between the `change graphic effect by`{:class="block3looks"} blocks, otherwise, it will happen so fast that you won't see it!

You can use a `clear graphic effects`{:class="block3looks"} block at any time to reset the effects:

```blocks3
clear graphic effects
```

--- /collapse ---

--- collapse ---
---
title: Click to change and then change back
---

You can add actions that make a change to a sprite and then reverse them, such as growing, waiting, and then shrinking.

**Squash ball when clicked**: [See inside](https://scratch.mit.edu/projects/435723273/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435723273/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

This code will grow a sprite, apply the `fisheye`{:class="block3looks"} effect for 0.5 seconds, and then return the sprite to its starting appearance:

```blocks3
when this sprite clicked
set size to (110)
set [fisheye v] effect to (50)
wait (0.5) seconds
set [fisheye v] effect to (0)
set size to (100)
```

--- /collapse ---

[[[scratch3-animate-movement-costumes]]]

### Backdrops

You can use code to change the backdrop too.

```blocks3
switch backdrop to ( v)

next backdrop

(backdrop [number v])
```

[[[scratch3-changing-backdrops-pages-levels]]]

### Visibility

The `show`{:class="block3looks"} and `hide`{:class="block3looks"} blocks control the visibility of a sprite.

```blocks3
show 

hide
```

[[[scratch3-show-hide-sprites-backdrops]]]

### Layers

To change how your sprites appear in relation to each other, you can use layers.

```blocks3
go to [front v] layer

go [forward v] () layers
```

[[[scratch3-positioning-with-layers]]]

--- collapse ---
---
title: Position sprites in many layers
---

**Through the window with tree**: [See inside](https://scratch.mit.edu/projects/454188775/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/454188775/?autostart=false" frameborder="0"></iframe>
</div>

In the example, the **Window frame** sprite appears at the front and the **Sun** sprite appears at the back. The **Avery Walking** and **Tree** sprites are each in their own layers between the **Window frame** sprite and the **Sun** sprite.

Use the `go backward`{:class="block3looks"} `1` `layers`{:class="block3looks"} block to place a sprite one layer behind the sprite at the front:

``` blocks3
when green flag clicked
go to [front v] layer
+go [backward v] (1) layers
```

Change the value in the `go backward`{:class="block3looks"} `1` `layers`{:class="block3looks"} block for each sprite, depending on where you want it to be positioned in relation to other sprites:

``` blocks3
when green flag clicked
go to [front v] layer
+go [backward v] (2) layers
```

--- /collapse ---

