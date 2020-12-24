## Debugging

<mark>Basic tips from Rik's Scratch debugging presentation / blog post but updated for Scratch 3
https://docs.google.com/document/d/1j1s9cEr-hlG0MIClhcLifnus5QlSmlw32imM81LJv_4/edit
</mark>

**Debugging** is finding and fixing mistakes in your code that are called **bugs**.

--- task ---

--- collapse ---
---

title: Debugging tips

---

+ **My sprite is going upside down** — Add a `set rotation style [left-right v]`{:class="block3motion"} or `set rotation style [don't rotate v]`{:class="block3motion"} block.

+ **My sprite 'jumps' when it changes costume or bounces** — Make sure that the costume is centered in the Paint editor (line up the blue cross with the cross hairs in the centre of the Paint editor).

+ **My sprite stops when it gets to the edge of the Stage** — Add an `if on edge, bounce`{:class="block3motion"} block.

+ **My sound does not play** — Have you added a block to `play sound`{:class="block3sound"} when the sprite is clicked? If you have copied code from another sprite, you will need to add the sound to this sprite from the `Sounds`{:class="block3sound"} tab. Check the volume on your computer and make sure that you have not lowered the volume with code — try `set volume to (100)%`{:class="block3sound"}.

+ **Other sprites keep going in front of my sprite** — Use a `go to [front v] layer`{:class="block3looks"} block.

+ **My sprite only moves/changes once** — Put your code inside a `forever`{:class="block3control"} block so it keeps running.

+ **My sprite does not change when I move a variable slider** — Put your code inside a `forever`{:class="block3control"} block so it keeps updating. 

--- /collapse ---

--- /task ---

--- task ---

**Tip**: Keep running your project to test your new code. Is it running as you imagined?

**Tip:** It's easier to identify issues if you make one change at a time and then run your program.

**Tip**: It might take a few experiments to get suitable behaviour for your sprite.

--- /task ---

--- save ---
