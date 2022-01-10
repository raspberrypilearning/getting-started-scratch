## Moje bloki

`Moje bloki`{:class="block3myblocks"} umożliwiają tworzenie nowych bloków dla duszka. Nadajesz blokowi nazwę, a następnie używasz `definiuj`{:class="block3myblocks"} do określenia co robi nowy blok, używając innych bloków Scratch. Możesz użyć swojego nowego bloku w dowolnym skrypcie na duszku, który zawiera ten bloku.

Ten przykład definiuje `talk`{:class="block3myblocks"}, który tworzy kostium zmiany duszka:

**Ćwierkający pingwin**: [Zajrzyj do środka](https://scratch.mit.edu/projects/567554899/editor){:target="_blank"}

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

Możesz użyć `Moje bloki`{:class="block3myblocks"}, aby **uporządkować** swój kod. Łatwiej jest zgrupować razem wszystkie bloki, dzięki którym duszek mówi, a następnie użyć jednego `talk`{:class="block3myblocks"}, gdy chcesz, aby twój duszek mówił.

Jeśli zdecydujesz, że chcesz zmienić sposób mówienia swojego duszka, wystarczy zmienić kod w jednym miejscu.

### Moje bloki z wejściami

Możesz również dodać **dane wejściowe** do bloków w sekcji `Moje bloki`{:class="block3myblocks"}, aby używały one wartości, które podajesz podczas korzystania z bloku.

**Pingwin mówi**: [Zajrzyj do środka](https://scratch.mit.edu/projects/567538874/editor){:target="_blank"}

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
title: Użyj Moich bloków do uporządkowania kodu
---
Najprostszym sposobem użycia menu `Moje bloki`{:class="block3myblocks"} jest pomoc w uporządkowaniu kodu. Oto prosty przykład.

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

`Moje bloki`{:class="block3myblocks"} są podobne do 'procedur', 'funkcji' lub 'metod' w innych językach programowania.
