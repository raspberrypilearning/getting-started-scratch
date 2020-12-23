## Miscellaneous dropdowns

--- task ---

Add code to make your sprite do something when it is clicked. You can pick one of these examples as a starting point.

--- collapse ---

--- 

title: Click to make sound and motion

---

You can make your sprite perform an action. It could play a sound or move when you click on it, and you can combine blocks to create a sequence of actions for the sprite to do every time you click on it. 

**Chirp and jump back when clicked**: [See inside](https://scratch.mit.edu/projects/435649420/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435649420/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

Add code blocks under a `when this sprite clicked`{:class="block3events"} block to run them when the sprite is clicked. This example plays a sound and move the sprite backwards. It can be used with a moving sprite. 

```blocks3
when this sprite clicked
play sound [chirp v] until done
move (-50) steps
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

This code will grow a sprite and apply the fisheye effect for one second and then return to normal:

```blocks3
when this sprite clicked
set size to (110)
set [fisheye v] effect to (50)
wait (0.5) seconds
set [fisheye v] effect to (0)
set size to (100)
```

--- /collapse ---

--- collapse ---
---

title: Click to make a change, reset with green flag

---
You can make your sprite change when you click on it, and then reset it when the green flag is clicked. 

**Balloon pop when clicked**: [See inside](https://scratch.mit.edu/projects/435725465/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435725465/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

This code makes a balloon 'pop' using `Sound`{:class="block3sound"} and `Looks`{:class="block3looks"} blocks. 

```blocks3
when this sprite clicked
change size by (10)
change [brightness v] effect by (25)
wait (0.1) seconds
play sound [pop v] until done
set [ghost v] effect to (100)
```

You need to make sure you also have set up code so that your balloon is not popped when you start your project:

```blocks3
when flag clicked
set size to (100)
clear graphic effects
```

--- /collapse ---

--- /task ---

--- task ---



--- /task ---
