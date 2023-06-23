## Мої блоки

`Мої блоки`{:class="block3myblocks"} дозволяють тобі створювати нові блоки для спрайта. Ти даєш блоку назву, а потім зможеш `визначати`{:class="block3myblocks"}, що буде робити новий блок, використовуючи інші блоки Scratch. Ти можеш використовувати свій новий блок в будь-якому скрипті на спрайті, який володіє цим блоком.

У цьому прикладі блок визначення `розмови`{:class="block3myblocks"} здійснює зміну образу спрайта:

**Щебетання пінгвіна**: [Переглянути код](https://scratch.mit.edu/projects/567554899/editor){:target="_blank"}

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

Ти можеш використовувати `Мої блоки`{:class="block3myblocks"}, щоб **організувати** свій код. Легше згрупувати всі блоки, які змушують спрайт говорити, а потім використовувати тільки один блок `talk`{:class="block3myblocks"}, коли хочеш, щоб твій спрайт заговорив.

Якщо ти захочеш змінити спосіб розмови свого спрайта, тобі потрібно буде змінити код лише в одному місці.

### Мої блоки з входами "Отримати"

Ти також можеш додати **входи "Отримати"** до `Мої блоки`{:class="block3myblocks"}, щоб вони використовували ті значення, які ти вказуєш при використанні блоку.

**Пінгвін розмовляє**: [Переглянути код](https://scratch.mit.edu/projects/567538874/editor){:target="_blank"}

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
title: Використовуй Мої блоки, щоб впорядкувати код
---
Найпростіший спосіб використання `Мої блоки`{:class="block3myblocks"} - це допомогти тобі впорядкувати код. Ось простий приклад.

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

`Мої блоки`{:class='block3myblocks'} подібні до 'процедур', 'функцій' або 'методів' в інших мовах програмування.
