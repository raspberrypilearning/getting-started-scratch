## Control

The blocks in the `Control`{:class="block3control"} blocks menu control the order that blocks run in, including decisions (selection) and loops (repetition).


The `wait`{:class="block3control"} block delays for a number of seconds before running the next block.

```blocks3
wait (1) seconds// delay for 1 second

wait (0.1) seconds// delay for one tenth of a second
```

Loops control how many time the code inside them runs.

```blocks3
repeat (4) // run the blocks inside four time

end
```

```blocks3
forever // run the blocks inside until stopped

end
```

[[[scratch3-forever-condition]]]

**Tip:** You can stop a `forever`{:class="block3events"} block by clicking the 'Stop' button above the stage. Or using the `stop`{:class="block3control"} blocks. 

There are three options for the `stop`{:class="block3events"} block:

```blocks3
stop [all] // stop all scripts in all sprites

stop [this script]

stop [other scripts in sprite]
```

The `if...then`{:class="block3control"} and `if...then...else` blocks are used to make decisions about which code blocks to run next. This is sometimes called **selection**. The `if...then`{:class="block3control"} block checks a hexagonal shaped **condition** and runs the code blocks inside if the condition is **true**. The `if...then..else`{:class="block3control"} block also has a section for code blocks to run if the condition is **false**.are

```blocks3
if <> then

end

if <> then

else

end
```

[[[scratch3-if-then-else]]]

You can find hexagonal shaped blocks to use as conditions in the `Operators`{:class="block3operators"} and `Sensing`{:class="block3sensing"} blocks menus.

The `wait until`{:class="block3control"} and `repeat until`{:class="block3control"} blocks also use conditions:

```blocks3
wait until <> // delay until the condition is true


repeat until <> // repeat the blocks inside until the condtion is true

end
```




