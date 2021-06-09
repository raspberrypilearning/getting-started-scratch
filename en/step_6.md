## Motion

`Motion`{:class="block3motion"} blocks allow you to move your sprite around the Stage. 

### Movement

```blocks3
move [10] steps
```

You can `go to`{:class="block3motion"} or `glide to`{:class="block3motion"} the mouse pointer, a random position on the Stage (or your finger on a tablet) or another sprite:

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

**Tip:** When you drag a sprite on the Stage, the motion blocks that use `x`{:class="block3motion"} and `y`{:class="block3motion"} coordinates update in the `Motion`{:class="block3motion"} blocks menu. The current `x`{:class="block3motion"} and `y`{:class="block3motion"} coordinates are show in the sprite pane.

### Rotation
You can also change the `direction`{:class="block3motion"} that a sprite is pointing in. This changes the direction that the sprite will move in if you use a `move`{:class="block3motion"} block. It may also change the rotation of the sprite's costume depending on the `rotation-style`{:class="block3motion"} setting.

Directions: 0 is up, 90 is right, 180 is down and 270 is left.

```blocks3
turn right [15] degrees

turn left [15] degrees

point in direction [90] // Click on 90 and drag the arrow to change

point towards (mouse-pointer v)

(direction)

set rotation style [left-right v] // or all-around or none
```

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

**Tip:** If you do not add a `move`{:class="block3motion"} block, your sprite will spin in the position that it is in. 

--- /collapse ---

--- collapse ---
---

title: Move in a circle

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

**Tip:** If you want your sprite to always start in the centre of the Stage, you can add a `go to x:`{:class="block3motion"} `0` `y:`{:class="block3motion"} `0` block before the `forever`{:class="block3control"} block. 

--- /collapse --- 

### Bouncing

The `if on edge, bounce`{:class="block3motion"} block is really useful when you want to make a sprite bounce around and stay on the Stage:

```blocks3
if on edge, bounce
```

See some of the ways in which you can get your sprite to move:

[[[scratch3-animate-movement-costumes]]]

--- collapse ---
---

title: Bounce on the edge of the Stage

---
--- no-print ---

**Girl moving across the Stage**: [See inside](https://scratch.mit.edu/projects/433535326/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433535326/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

This code makes a sprite bounce on the left-hand and right-hand edges of the Stage. Because the sprite rotates horizontally, it appears to flip when it changes its direction when the green flag is clicked:

```blocks3
when green flag clicked
point in direction (90)
set rotation style [left-right v]
forever
move (5) steps
if on edge, bounce
```

In this example, the `point in direction`{:class="block3motion"} block automatically points the sprite to the right (`90` degrees) when the green flag is clicked. If you change the number of degrees to `-90`, your sprite will point left.

Add a `set rotation style`{:class="block3motion"} block and select `left-right`{:class="block3motion"} in the drop-down menu, so that your sprite will not flip upside down when it bounces on the edge of the Stage. 

**Tip:** You can drag your sprite on the Stage to move it to the y (up–down) position that you want.

--- /collapse ---

--- collapse ---
---

title: Bounce up and down the Stage

---
--- no-print ---

**Girl jumping**: [See inside](https://scratch.mit.edu/projects/433595822/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433595822/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

This code makes a sprite bounce up and down the Stage when the green flag is clicked:

```blocks3
when green flag clicked
point in direction (0)
set rotation style [don't rotate v]
forever
move (5) steps
if on edge, bounce
```

Change the number of degrees in the `point in direction`{:class="block3motion"} block to `0` to make a sprite point upwards.

Add a `set rotation style`{:class="block3motion"} block and select `don't rotate`{:class="block3motion"} in the drop-down menu to stop your sprite rotating, even when it bounces.

**Tip:** You can drag your sprite around the Stage to move it to the x (left–right) position that you want.

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

This code makes a sprite appear to rotate randomly when the green flag is clicked:

```blocks3
when green flag clicked
point in direction (45)
set rotation style [all around v]
forever
move (5) steps
if on edge, bounce
```

If your sprite moves at `45` degrees, you will find that it appears to bounce on the edge of the Stage at an angle. Change the number of degrees in the `point in direction`{:class="block3motion"} block to `45` to make your sprite bounce all around.

Add a `set rotation style`{:class="block3motion"} block and select `all around`{:class="block3motion"} in the drop-down menu, so that your sprite will turn when it bounces on the edge of the Stage.  

--- /collapse ---

### Using coordinates

You can also `change`{:class="block3motion"} and `set`{:class="block3motion"} the `x`{:class="block3motion"} and `y`{:class="block3motion"} coordinates and get their values to use in other blocks:

[[[generic-scratch3-coordinates]]]

```blocks3 
change x by [10]

set x to [0]

change y by  [10]

set y to [0]

(x position)

(y position)
```
