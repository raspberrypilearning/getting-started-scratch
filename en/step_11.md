## Debug

**Debugging** is finding and fixing mistakes in your code that are called **bugs**.

* It's easier to identify issues if you make one change at a time and then run your program.

* It might take a few experiments for your project to work in the way you planned.

Here are some tips that can help you to debug a project when it is not doing what you want it to do:

--- collapse ---
---
title: Run smaller pieces of code
---

You do not have to run a whole program to check whether the last few new blocks that you have added work.

* Click on a block in the **Code area** to run it — it is a quick way to check that a block is working as you expect it to.

* To test a set of blocks on their own, drag them away from their **containing** script, click on them to test them, then drag them back to the main script.

--- /collapse ---

--- collapse ---
---
title: Add temporary delays
---

Slow down the **execution** of your code when it is run. To do this, add a `wait`{:class="block3control"} or `wait until key pressed`{:class="block3control"} block, then remove the block when you have finished debugging your code.

--- /collapse ---

--- collapse ---
--- 
title: Show variables on the Stage
---

If your project uses `variables`{:class="block3variables"} to store data, then it can be helpful to show those `variables`{:class="block3variables"} on the Stage. 

Click on the checkbox next to a `variable`{:class="block3variables"} in the `Variables`{:class="block3variables"} blocks menu to show or hide it on the Stage. 

Does the variable always have the value that you expect?

--- /collapse ---

--- collapse ---
---
title: Add comments
---

Add comments to blocks, sets of blocks, and/or scripts. Use everyday language to explain what the code does. Sometimes, this will make you realise that your code does not actually do what you want it to do!

Comments are useful for when you want to understand your code later, and they help other people to understand your projects.

--- /collapse ---


There are common problems that lots of beginners (and experts!) experience in Scratch. 

--- collapse ---
---

title: Debugging tips for specific problems

---

+ **My sprite is going upside down** — Add a `set rotation style left-right`{:class="block3motion"} or `set rotation style don't rotate`{:class="block3motion"} block.

+ **My sprite 'jumps' when it changes costume or bounces** — Make sure that the costume is centred in the Paint editor (line up the blue cross with the crosshair in the centre of the Paint editor).

+ **My sprite stops when it gets to the edge of the Stage** — Add an `if on edge, bounce`{:class="block3motion"} block.

+ **My sound does not play** — Have you added a block to `play sound`{:class="block3sound"} when the sprite is clicked? If you have copied code from another sprite, you will need to add the sound to this sprite from the **Sounds** tab. Check the volume on your computer and make sure that you have not lowered the volume with code — try `set volume to`{:class="block3sound"}`100`.

+ **Other sprites keep going in front of my sprite** — Use a `go to front layer`{:class="block3looks"} block.

+ **My sprite only moves/changes once** — Put your code inside a `forever`{:class="block3control"} block so it keeps running.

+ **My sprite does not change when I move a variable slider** — Put your code inside a `forever`{:class="block3control"} block so it keeps updating. 

--- /collapse ---

**Tip**: If you cannot find the problem after you have tried these techniques, then take a break or work on a different part of your project. When you come back, you might find the bug straight away!

