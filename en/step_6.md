## Motion

--- task ---

`Motion`{:class="block3motion"} blocks allow you to move your sprite so that it can bounce and/or spin around the Stage. See some of the ways in which you can get your sprite to move:

--- collapse ---
---
title: Move your sprite
---

Get your sprite to `move`{:class="block3motion"}:

```blocks3
when green flag clicked
point in direction (90)
set rotation style [left-right v]
forever
move (5) steps
if on edge, bounce
```
--- /collapse ---

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

This code makes a sprite bounce on the left-hand and right-hand edges of the Stage. Because the sprite rotates horizontally, it appears to flip when changing its direction when the green flag is clicked:

```blocks3
when green flag clicked
point in direction (90)
set rotation style [left-right v]
forever
move (5) steps
if on edge, bounce
```

In this example, the `point in direction`{:class="block3motion"} block automatically points your sprite to the right (`90` degrees) when the green flag is clicked. If you change the number of degrees to `-90`, your sprite will point left.

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

If your sprite moves at `45` degrees, you will find that it appears to bounce on the edge of the Stage in a random direction. Change the number of degrees in the `point in direction`{:class="block3motion"} block to `45` to make your sprite bounce all around.

Add a `set rotation style`{:class="block3motion"} block and select `all around`{:class="block3motion"} in the drop-down menu, so that your sprite will turn when it bounces on the edge of the Stage.  

--- /collapse ---

--- collapse ---
---

title: Spin around

---
--- no-print ---

**Bat spinning**: [See inside](https://scratch.mit.edu/projects/435704980/editor){:target="_blank"}

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

This code makes a sprite fly in a circle when it is clicked:

```blocks3
when green flag clicked
forever
move (1) steps
turn right (1) degrees :: motion
```

Change the values in a `move`{:class="block3motion"} block and `turn`{:class="block3motion"} block within a `forever`{:class="block3control"} loop to `1` and your sprite will appear to move in a big circle.

**Tip:** If you want your sprite to always start in the centre of the Stage, you can add a `go to x:`{:class="block3motion"}`0``y:`{:class="block3motion"}`0` block before the `forever`{:class="block3control"} block. 

--- /collapse --- 

--- /task ---

--- task ---
+ Drag your sprite to a different starting position on the Stage.
+ Increase the number of steps in a `move`{:class="block3motion"} block to make your sprite move faster, or decrease the number to make your sprite move slower.
+ Change the number of degrees in a `point in direction`{:class="block3motion"} block to change the direction that your sprite starts to move in. 
+ Change the number of degrees in a `turn right`{:class="block3motion"} or `turn left`{:class="block3motion"} block so that your sprite turns faster or slower. 
+ Combine `move`{:class="block3motion"} and `turn right`{:class="block3motion"} or `turn left`{:class="block3motion"} blocks so that your sprite moves and turns. 
+ Experiment with the `set rotation style`{:class="block3motion"} block to make sure that you understand what the different options do.
--- /task ---
