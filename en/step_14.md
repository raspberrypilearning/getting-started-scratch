## My blocks

`My blocks`{:class="block3myblocks"} allow you to create new blocks for a sprite. You give the block a name and then `define`{:class="block3myblocks"} what the new block does using other Scratch blocks. You can use your new block in any script on the sprite that owns the block.

This example defines a `talk`{:class="block3myblocks"} block that makes a sprite change costume:

**Penguin chirps**: [See inside](https://scratch.mit.edu/projects/567554899/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567554899/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

```blocks3
define talk
switch costume to (penguin2-b v)
repeat (2)
play sound (chirp v) until done
end
switch costume to (penguin2-a v)

when this sprite clicked
talk

when [space v] key pressed
talk
```

You can use `My blocks`{:class="block3myblocks"} to **organise** your code. It's simpler to group together all the blocks that make a sprite talk and then just use one `talk`{:class="block3myblocks"} block when you want your sprite to talk.

If you decide that you want to change the way your sprite talks then you only have to change the code in one place. 

### My blocks with inputs

You can also add **inputs** to `My blocks`{:class="block3myblocks"} so that they use the values you provide when you use the block.

**Penguin talks**: [See inside](https://scratch.mit.edu/projects/567538874/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567538874/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

```blocks3
define talk (words)
switch costume to (penguin2-b v)
say (words) // use the provided input
repeat (2)
play sound (chirp v) until done
end
say (words)
switch costume to (penguin2-a v)

when this sprite clicked
talk [hello]

when [space v] key pressed
talk [hi]
```

[[[generic-scratch3-make-block]]]

--- collapse ---
---
title: Use My Blocks to organise code
---
The simplest way to use My Blocks{:class="block3myblocks"} is to help organise your code. Here is a simple example.

```blocks3
define move right
if <not <touching (edge v) ?>> then
switch costume to [right_1 v]
change x by (2)
switch costume to [right_2 v]
change x by (2)
switch costume to [right_3 v]
change x by (2)
end

define move left
if <not <touching (edge v) ?>> then
switch costume to [left_1 v]
change x by (-2)
switch costume to [left_2 v]
change x by (-2)
switch costume to [left_3 v]
change x by (-2)
end

when flag clicked
forever
if <key (right arrow v) pressed> then
move right
end
if <key (left arrow v) pressed> then
move left
```

--- /collapse ---

`My blocks`{:class="block3myblocks"} are similar to 'procedures', 'functions' or 'methods' in other programming languages.
