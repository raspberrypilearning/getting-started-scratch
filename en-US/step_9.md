## Events

Blocks in the `Events`{:class="block3events"} menu control when scripts are started.

**Hat blocks** run the blocks below them when a particular event happens. They are rounded at the top, like a hat, so no blocks can go above them.

You can use:

```blocks3

when flag clicked // run blocks when the green flag above the Stage is clicked

when this sprite clicked // run the blocks when the sprite for this script is clicked

when stage clicked // run the blocks when the stage is clicked

```

**Tip:** The `when stage clicked`{:class="block3events"} block is only available when you are working in the Code area for the Stage.

If you are on a computer with a keyboard, you can use `when key pressed`{:class="block3events"}:

```blocks3
when [space v] key pressed // change to number, letter or arrow keys
```

You can also use a `when backdrop switches to`{:class="block3events"} block to start a script when the backdrop changes.

[[[scratch3-changing-backdrops-pages-levels]]]

[[[scratch3-show-hide-sprites-backdrops]]]


The `when >`{:class="block3events"} block has two versions:

```blocks3
when [loudness v] > (10) // run blocks when the microphone detects sound

when [timer v] > (10) // run blocks when the timer reaches 10 seconds
```

[[[scratch3-time-delay]]]


The last two blocks in the `Events`{:class="block3events"} menu are `broadcast`{:class="block3events"} blocks. You can use `when i receive (message v)`{:class="block3events"} to start a script when any sprite runs a matching `broadcast (message v)`{:class="block3events"} block.

[[[generic-scratch3-broadcast-message]]]

