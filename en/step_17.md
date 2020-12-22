## Looks

--- task ---

Add code to your sprite to change the way it looks. Only make changes to your sprite if it makes sense. If you are already happy with the way your sprite looks, you can move on to the next task.

You can use these examples to get started:

--- collapse ---
---
title: Set size
---

When you add a sprite to your project its size is set to `100` percent. This may be too big or too small for your project. 

You can use code to set the size of a sprite. 

```blocks3
set size to (50) %
```

If you set the size of a sprite to `50` percent, it will be half as tall and half as wide. If you set the size of a sprite to `200` percent, it will be twice as tall and twice as wide. 

Place a `set size`{:class="block3looks"} block under a `when green flag clicked`{:class="block3events"} block to set the size of a sprite when the project is started: 

```blocks3
when green flag clicked
set size to (50) %
```

You can also quickly set the size of a sprite using the **Size** button underneath the Stage:

![Sprite Size setting highlighted](images/spriteSize.png){:width="400px"}

--- /collapse ---

--- collapse ---
---
title: Set graphic effects
---

**Rooster effects**: [See inside](https://scratch.mit.edu/projects/435730522/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/435730522/?autostart=false" frameborder="0"></iframe>
</div>

Place a `set graphic effects`{:class="block3looks"} block under a `when green flag clicked`{:class="block3events"} block to set the size of a sprite when the project is started:

```blocks3
when green flag clicked
set [ghost v] effect to (25)
```

The `set color`{:class="block3looks"} and `color`{:class="block3looks"} blocks both have drop-down boxes where you can choose from a range of different graphic effects that can be used to change your sprite's appearance.

+ `color`{:class="block3looks"}: From 0 to 199 (bigger numbers will wrap around, so 200 is the same as 0)
+ `fisheye`{:class="block3looks"}: 0 is no effect, bigger numbers give a bigger 'bulge' effect
+ `whirl`{:class="block3looks"}: 0 is no effect, big number gives a big whirl to the left, big negative number gives a big whirl to the right
+ `pixelate`{:class="block3looks"}: 0 is no effect, bigger numbers create more pixels
+ `mosaic`{:class="block3looks"}: 0 is no effect, bigger numbers create more copies
+ `brightness`{:class="block3looks"}: 0 is no effect, bigger numbers up to 100 make the sprite lighter, and negative numbers down to -100 make the sprite darker 
+ `ghost`{:class="block3looks"}: 0 is no effect, bigger numbers up to 100 make the sprite more transparent 

Try `setting`{:class="block3looks"} the different effect values to see what each one does. Explore how different value changes make your sprite look.

```blocks3
set [whirl v] effect to (100)

set [pixelate v] effect to (50)
```

--- /collapse ---

--- collapse ---
---
title: Use the Fill tool to change the colours in a costume
---

Select your sprite under the Stage and then click on **Costumes**. 

Change the colour of your sprite. Click on the second sprite in the Sprite menu. Then select its **Costumes** tab.

Use the **Arrow** tool to highlight whichever part of the costume you want to change colour.

![Image showing Arrow tool in Paint editor](images/challenge1-arrow-tool.png){:width="200px"}

![Image showing Arrow tool selecting shape](images/challenge1-arrow-tool-selecting-shape.png){:width="300px"}

Go to the **Fill** tool and select the colour. It will automatically fill the shape that you have selected.

![Image showing Fill tool in Paint editor](images/challenge1-fill-tool.png){:width="300px"}

Repeat the steps above with any part of the costume you have missed or for any other part of the costume you want to change the colour of.

![Image showing shape colour changing](images/challenge1-select-another-shape.png){:width="300px"}

![Image showing shape colour changing](images/challenge1-change-shape-colour.png){:width="300px"}

![Image showing final change](images/challenge1-change-costume-colour.png){:width="300px"}


--- /collapse ---

--- /task ---
