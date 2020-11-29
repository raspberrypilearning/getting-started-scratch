## Useful Code

<mark>Relevant code snippets as in Code Club book. 
https://www.raspberrypi.org/magpi-issues/CC_Book_of_Scratch_v1.pdf
(Some but not all of those plus any others that make sense for projects 1-3) Would also link to relevant skills projects to those who arrive on this page via search/browse.</mark>

Try changing the numbers and drop-down options in these useful scripts to get different effects. Combine multiple scripts and use looks blocks. 

Remember, you can add code to sprites and to the Stage. 

### Playing a sound

```blocks3
when this sprite clicked
play sound [pop v] until done
```

### Spinning sprite

```blocks3
when flag clicked
forever
turn right (1) degrees
```

### Animating sprite costumes

```blocks3
when flag clicked
forever
next costume
wait (0.1) seconds
```

### Bouncing sprite

```blocks3
when flag clicked
point in direction (90)
set rotation style [left-right v]
forever
move (1) steps
if on edge, bounce
```

### Change when clicked

```blocks3
when this sprite clicked
next costume
```

Or,

```blocks3
when this sprite clicked
change [colour v] effect by (25)
```

### Change and change back

```blocks3
when this sprite clicked
set [fisheye v] effect to (20)
wait (1) seconds
clear graphic effects
```

Or, you can `play sound until done`{:class="block3sounds"} instead of using `wait`{:class="block3control"}. 


### Keep changing

```blocks3
when flag clicked
forever
set size to (110)%
set [brightness v] effect to (20)
wait (0.25) seconds
set size to (100)%
set [brightness v] effect to (0)
wait (0.25) seconds
```

### Move in a circle

```blocks3
when flag clicked
forever
move (1) steps
turn right (1) degrees
```


### Update a block with a variable

```blocks3
when flag clicked
forever
set [color v] effect to (my variable)
```

### Program sprites into layers

```blocks3
when flag clicked
go to [front v] layer
go back (1) layers
```







