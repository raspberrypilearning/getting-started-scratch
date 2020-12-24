## What is what in Scratch

--- task ---
**Sprites** are characters and objects that appear on the stage which can be controlled by Scratch blocks, including being moved.

Sprites may have multiple **costumes**. Changing the costume changes the appearance of a sprite, and can be used for effects such as giving the appearance of walking.

The **Stage** is the area where the sprites are active in Scratch. The Stage can have backdrops and can be controlled using Scratch blocks but the Stage cannot move.

**Backdrop**. The stage can have a backdrop or even mulitple backdrops. Changing the backdrop can be used for effects such as changing the location in a story, or moving onto a new level of a game.

**code** is made up of Scratch blocks that give instructions to the sprites and the stage to perform a certain function, such as moving around the stage. 

--- /task ---

--- task ---

**Blocks** refer to the visual code blocks that are put together in Scratch to give instructions to the stage and the sprites.

There are colour coded categories of blocks: `Motion`{:class="block3motion"}, `Looks`{:class="block3looks"}, `Sound`{:class="block3sound"}, `Events`{:class="block3events"}, `Control`{:class="block3control"}, `Sensing`{:class="block3sensing"}, `Operators`{:class="block3operators"}, `Variables`{:class="block3variables"}, and `My Blocks`{:class="block3myblocks"}. There are also most blocks in `Extensions`{:class="block3extensions"}.

You can drag blocks together to make programs - as you drag them towards each other they snap together.

**Hat blocks** start code running when a particular event happens.`Event`{:class="block3events"} blocks like `when green flag clicked`{:class="block3events"} to run your program start all scripts. `Event`{:class="block3events"} blocks have a runded top shape which means you cannt add a block above them. You always need an `Event`{:class="block3events"} block for **when** your sprite or backdrop does something. `Event`{:class="block3events"} blocks start code running when a particular event happens, such as `when this sprite clicked`{:class="block3events"}.

```blocks3
when green flag clicked
when this sprite clicked
```

**Tip**: When you are developing your programs you can click on the code blocks to run them. 

A **script** is a series of blocks that are joined together to give instructions to the stage or sprites. The stage and sprites may each have many different scripts.

Some blocks have **input** ranges. For instance, in the `Looks`{:class="block3looks"} blocks:

```blocks3
set size to (100)%
```

100% is the normal size (edit the costume to change how big this is).
50% is half the normal size
200% is double the normal size

Some blocks have **drop-down** options and **input** ranges. For instance, in the `Looks`{:class="block3looks"} blocks:

```blocks3
set [color v] effect to (100)
```

+ `color`{:class="block3looks"}: from 0 to 199 (bigger numbers will wrap around so 200 is the same as 0)
+ `fisheye`{:class="block3looks"}: 0 is no effect and bigger numbers give a bigger 'bulge' effect
+ `whirl`{:class="block3looks"}: 0 is no effect, big number give a big whirl to the left, big negative number give a big whirl to the right
+ `pixelate`{:class="block3looks"}: 0 is no effect, bigger numbers give more pixels
+ `mosaic`{:class="block3looks"}: 0 is no effect, bigger numbers create more copies
+ `brightness`{:class="block3looks"}: 0 is no effect, bigger numbers up to 100 make the sprite lighter and negative numbers down to -100 make the sprite darker 
+ `ghost`{:class="block3looks"}: 0 is no effect, bigger numbers up to 100 make the sprite more transparent

**Loops** are blocks that make code repeat itself in a loop. The most simple repeat loop `forever`{:class="block3control"} repeats the code inside it forever (until the programme is stopped). Another useful loop is `repeat until`{:class="block3control"} which repeats the code inside it a set number of times.

```blocks3
forever
repeat until ()
```
--- /task ---
