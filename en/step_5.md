## Useful Code

Relevant code snippets as in Code Club book. 
https://www.raspberrypi.org/magpi-issues/CC_Book_of_Scratch_v1.pdf
(Some but not all of those plus any others that make sense for projects 1-3)

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





