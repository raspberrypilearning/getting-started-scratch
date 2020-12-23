## Motion

--- task ---

Add code to make your sprite bounce and/or spin around the Stage in the way you want it to. 

If you need a reminder about how to create your sprite's movement when it bounces on the edge of the Stage, then click the below for **Information**.

--- collapse ---
---

title: Bounce across the Stage

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

The `point in direction`{:class="block3motion"} block automatically points your sprite to the right (`90` degrees) when the green flag is clicked. If you change the number of degrees to `-90`, your sprite will point left.

Add a `set rotation  style`{:class="block3motion"} block and select the drop-down `left-right`{:class="block3motion"} so your sprite won't flip upside down when it bounces off the edge of the Stage.  

**Tip:** You can drag your sprite on the Stage to move it to the y (up-down) position that you want.

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

Change the number of degrees in the `point in direction`{:class="block3motion"} block to `0` to make a sprite point upwards when the green flag is clicked.

Add a `set rotation  style`{:class="block3motion"} block and select the drop-down `don't rotate`{:class="block3motion"} block to stop your sprite rotating, even when it bounces.

**Tip:** You can drag your sprite around the Stage to move it to the x (left-right) position that you want.

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

If your sprite moves at `45` degrees, you will find it appears to bounces off the edge of the Stage in a random direction. Change the number of degrees in the `point in direction`{:class="block3motion"} block to `45` to make a sprite bounce all around.

Add a `set rotation  style`{:class="block3motion"} block and select the drop-down `all around`{:class="block3motion"} block, so your sprite will turn when it bounces off the edge of the Stage.  

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

This code makes a sprite spin when it is clicked:

```blocks3
when flag clicked
forever
turn right (1) degrees :: motion
```

Change the degrees by which your sprite turns to `1` within a `forever`{:class="block3control"} loop and your sprite will appear to spin.

**Tip:** If you don't add a `move`{:class="block3motion"} block, your sprite will spin in the position its in. 

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

Change the degrees by which your sprite `moves`{:class="block3motion"} to `1` and `turns`{:class="block3motion"} to `1` within a `forever`{:class="block3control"} loop and your sprite will appear to move in a big circle.

**Tip**: If you want your sprite to always start in the centre of the Stage, you can add `go to x:(0) y: (0)`{:class="block3motion"} before the `forever`{:class="block3control"} block. 

--- /collapse --- 

--- /task ---

--- task ---
Remember to keep running your project to test it. Is the program working as you had planned?

It might take a few experiments to get suitable behaviour for your sprite.

You could:
+ Drag your sprite to a different starting location on the Stage.
+ Increase the number of steps in `move ( ) steps`{:class="block3motion"} to make your sprite move faster, or decrease it to move slower.
+ Change the number of degrees in `point in direction ( )`{:class="block3motion"} to change the direction that your sprite starts to move in. 
+ Change the number of degrees in `turn right`{:class="block3motion"} or `turn left`{:class="block3motion"} so that your sprite turns faster or slower. 
+ Combine `move ( ) steps`{:class="block3motion"} and `turn right`{:class="block3motion"} or `turn left`{:class="block3motion"} so that your sprite moves and turns. 
+ Experiment with `set rotation style [ ]`{:class="block3motion"} to make sure you understand what the different options do.

**Tip:** It's easier to identify issues if you make one change at a time and then run your program.

--- /task ---
