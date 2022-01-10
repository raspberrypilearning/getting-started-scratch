## Fy Mlociau

Mae `Fy Mlociau`{:class="block3myblocks"} yn gadael i ti greu blociau newydd ar gyfer corlun. Rwyt ti'n rhoi enw i'r bloc ac wedyn yn `diffinio`{:class="block3myblocks"} beth mae'r bloc newydd yn ei wneud gan ddefnyddio blociau Scratch eraill. Galli di ddefnyddio dy floc newydd mewn unrhyw sgript ar y corlun sy'n berchen ar y bloc.

Mae'r enghraifft hon yn diffinio bloc `siarad`{:class="block3myblocks"} sy'n gwneud i gorlun newid ei wisg:

**Pengwin yn trydar**: [See inside](https://scratch.mit.edu/projects/567554899/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567554899/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

```blocks3
define siarad
switch costume to (penguin2-b v)
repeat (2)
play sound (chirp v) until done
end
switch costume to (penguin2-a v)

when this sprite clicked
siarad

when [space v] key pressed
siarad
```

Galli di ddefnyddio `Fy mlociau`{:class="block3myblocks"} i **drefnu** dy god. Mae'n haws grwpio'r holl flociau sy'n gwneud i gorlun siarad gyda'i gilydd ac wedyn defnyddio un bloc `siarad`{:class="block3myblocks"} pan rwyt ti am i dy gorlun siarad.

Os byddi di'n penderfynu dy fod am newid y ffordd mae dy gorlun yn siarad yna dim ond mewn un lle mae'n rhaid i ti newid y cod.

### Fy mlociau gyda mewnbynnau

Galli di ychwanegu **mewnbynnau** i `Fy mlociau`{:class="block3myblocks"} fel eu bod yn defnyddio'r gwerthoedd byddi di'n eu darparu pan rwyt ti'n defnyddio'r bloc.

**Pengwin yn siarad**: [See inside](https://scratch.mit.edu/projects/567538874/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567538874/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

```blocks3
define siarad (geiriau)
switch costume to (penguin2-b v)
say (geiriau) // defnyddio'r mewnbwn a roddwyd
repeat (2)
play sound (chirp v) until done
end
say (geiriau)
switch costume to (penguin2-a v)

when this sprite clicked
siarad [helo]

when [space v] key pressed
siarad [haia]
```

[[[generic-scratch3-make-block]]]

--- collapse ---
---
title: Defnyddio Fy Mlociau i drefnu cod
---
Y ffordd symlaf o ddefnyddio `Fy Mlociau`{:class="block3myblocks"} yw i helpu drefnu dy god. Dyma enghraifft syml.

```blocks3
define symud i'r dde
if <not <touching (edge v) ?>> then
switch costume to [right_1 v]
change x by (2)
switch costume to [right_2 v]
change x by (2)
switch costume to [right_3 v]
change x by (2)
end

define symud i'r chwith
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
symud i'r dde
end
if <key (left arrow v) pressed> then
symud i'r chwith
```

--- /collapse ---

Mae `Fy Mlociau`{:class="block3myblocks"} yn debyg i 'weithdrefnau', 'ffwythiannau' neu 'ddulliau' mewn ieithoedd rhaglennu eraill.
