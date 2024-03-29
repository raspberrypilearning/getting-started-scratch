## Sound

To add sound to your project, use `Sound`{:class="block3sound"} blocks. For example, you can create a continuous background soundtrack, or add sounds that play at regular intervals.

![An annotated screenshot of the Sounds tab.](images/Scratch-Sound-tab.png){:width="600px"}

First, select a sound from the Sound Library, or record your own sound.

[[[scratch3-add-sound]]]
 
[[[scratch3-record-sound]]]

Add code to run `Sound`{:class="block3sound"} blocks where you want sound in your project.
  
--- collapse ---
---
title: Add a long sound to create a continuous soundtrack
---
 
Click on the green flag to hear the sounds.

**Radio soundtrack**: [See inside](https://scratch.mit.edu/projects/444581851/editor){:target="_blank"}
 
<div class="scratch-preview">
 <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/444581851/?autostart=false" frameborder="0"></iframe>
</div>
 
You can use a `play sound until done`{:class="block3sound"} block inside a `forever`{:class="block3control"} loop. Once the sound has finished, the `forever`{:class="block3control"} loop makes the sound start again from the beginning.

This code uses a single long sound clip repeated as a soundtrack:
 
```blocks3
when green flag clicked
forever
play sound (Dance Snare Beat v) until done
end
```

**Note:** When you choose a new sound, if you select the **Loops** category, Scratch will only show you the sounds that are suitable for a single looping soundtrack.

![The 'Loops' category in the Sound Library.](images/loopSounds.png)

--- /collapse ---
 
--- collapse ---
---
title: Add a sequence of short sounds to create a continuous soundtrack
---
  
Click on the green flag to hear the sounds. 

**Champ performance**: [See inside](https://scratch.mit.edu/projects/444673165/editor){:target="_blank"}
 
<div class="scratch-preview">
 <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/444673165/?autostart=false" frameborder="0"></iframe>
</div>

 Use a `forever`{:class="block3control"} block to create a looped sound. You can:
+ Put a series of short sounds in a sequence, or 
+ Use different instrument notes and effects
 
```blocks3
when flag clicked
forever
play sound (Low Boing v) until done
play sound (Low Boing v) until done
play sound (Drum Buzz v) until done
play sound (Pop v) until done
play sound (Bird v) until done
play sound (Bark v) until done
play sound (Glug v) until done
End
```
  
--- /collapse ---
 
--- collapse ---
---
title: Add sounds that play at regular intervals
---
 
**Football sounds**: [See inside](https://scratch.mit.edu/projects/450870079/editor){:target="_blank"}
 
Click on the green flag to hear the sounds. 

<div class="scratch-preview">
 <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/450870079/?autostart=false" frameborder="0"></iframe>
</div>
 
 In this project, the **Stage** has code to play a sound at regular intervals:

 ```blocks3
 when flag clicked
 forever
 wait (3) seconds
 play sound (Cheer v) until done
 end
 ```

The **Whistle** sprite also plays a sound at regular intervals:

 ```blocks3
 when this sprite clicked
 forever
 play sound (Referee Whistle v) until done
 wait (4) seconds
 end
 ```

--- /collapse ---

--- collapse ---
---
title: Add sounds that start to play at the same time
---

There are two `Sound`{:class="block3sound"} blocks with an important difference:

+ When you `play sound until done`{:class="block3sound"}, the sound will play all the way through. The next line of code in the script will not run until the sound has finished playing.

+ When you `start sound`{:class="block3sound"}, the sound will play, but the next block will run immediately and will not wait for the sound to finish playing first.

This means that if you had a series of `start sound`{:class="block3sound"} blocks, the sounds would all play almost at the same time, layered on top of each other. The effect can be interesting and sometimes messy.

Have a play with it sometime!

```blocks3
when green flag clicked
start sound (Meow v)
start sound (Alien Creak2 v)
start sound (Boing v)
start sound (Boom Cloud v)
start sound (Baa v)
```

--- /collapse ---
 
Once you have chosen your sounds, you may want to change the `volume`{:class="block3sound"}, `pitch`{:class="block3sound"}, or `pan`{:class="block3sound"} (so you hear the sound from the left- or right-hand speaker).

--- collapse ---
---
title: Volume, pitch, and pan
---

Click on the green flag to hear the sounds. 

**Band practice**: [See inside](https://scratch.mit.edu/projects/451697380/editor){:target="_blank"}

<div class="scratch-preview">
 <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/451697380/?autostart=false" frameborder="0"></iframe>
</div>

The **Drums** sprite uses `set volume to`{:class="block3sound"}, `set pitch effect to`{:class="block3sound"}, and `set pan left/right effect to`{:class="block3sound"} blocks to change the sound:

```blocks3
set volume to (80) %
set [pitch v] effect to (50) :: sound
set [pan left/right v] effect to (-100) :: sound
play sound (Drum Funky v) until done
```

+ You can `set volume to`{:class="block3sound"} a value from `0` (silent) to `100` (full volume). This is useful if you want some sounds to play louder than others, or if you want a sprite to appear further away.

+ The `pitch`{:class="block3sound"} effect controls how high or low a sound is. Setting the pitch to a higher value also makes a sound faster. You can `set pitch effect to`{:class="block3sound"} values between `-360` (very low) and `360` (very high).

+ The `pan left/right`{:class="block3sound"} effect allows you to control whether a sound comes out of a left- or right-hand speaker or headphone or both. You can `set pan left/right effect to`{:class="block3sound"} values from `-100` (all sound from the left) to `100` (all sound from the right).

--- /collapse ---

You can also use the `Text to Speech`{:class="block3extensions"} extension:

[[[scratch3-text-to-speech]]]

