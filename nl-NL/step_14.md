## Mijn blokken

Met `Mijn blokken`{:class="block3myblocks"} kun je nieuwe blokken maken voor een sprite. Je geeft het blok een naam en dan `definieer`{:class="block3myblocks"} je wat het nieuwe blok doet met gebruikmaking van andere Scratch blokken. Je kunt je nieuwe blok gebruiken in elk script op de sprite die eigenaar is van het blok.

Dit voorbeeld definieert een `praat`{:class="block3myblocks"} blok waardoor een sprite van uiterlijke verandert:

**Pinguïn piept**: [Bekijk van binnen](https://scratch.mit.edu/projects/567554899/editor){:target="_blank"}

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

Je kunt `Mijn blokken`{:class="block3myblocks"} gebruiken om jouw code te **organiseren**. Het is eenvoudiger om alle blokken bij elkaar te voegen die een sprite laten praten en dan gewoon een `praat`{:class="block3myblocks"} blok te gebruiken als je wilt dat je sprite praat.

Als je besluit dat je de manier waarop je sprite praat wilt veranderen, hoef je de code maar op één plek te wijzigen.

### Mijn blokken met invoer

Je kunt ook **invoer** voor `Mijn blokken`{:class="block3myblocks"} toevoegen, zodat ze de waarden gebruiken die je opgeeft wanneer je het blok gebruikt.

**Pinguïn praat**: [Bekijk van binnen](https://scratch.mit.edu/projects/567538874/editor){:target="_blank"}

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
titel: Mijn blokken gebruiken om code te ordenen
---
De eenvoudigste manier om `Mijn blokken`{:class="block3myblocks"} te gebruiken, is om je code te helpen organiseren. Hier is een eenvoudig voorbeeld.

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

`Mijn blokken`{:class="block3myblocks"} zijn vergelijkbaar met 'procedures', 'functies' of 'methoden' in andere programmeertalen.
