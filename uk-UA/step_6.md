## Рух

Блоки `Рух`{:class="block3motion"} призначені для того, щоб переміщати спрайт по Сцені.

### Переміщення

Блок `перемістити на`{:class="block3motion"} - це найпростіший спосіб почати переміщення спрайта:

```blocks3
move [10] steps
```

Ти можеш `перейти до`{:class="block3motion"} або `ковзати до`{:class="block3motion"} курсора миші (або пальця на планшеті), випадкового місця на Сцені, або до іншого спрайта:

```blocks3
go to (random position v)

glide [1] secs to (random position v)
```

Також ти можеш `перемістити в`{:class="block3motion"} або `ковзати до`{:class="block3motion"} позиції, яка задається координатами на Сцені `x`{:class="block3motion"} та `y`{:class="block3motion"}.

```blocks3
go to x: [0] y: [0] 

glide [1] secs to x: [0] y: [0]
```

[[[scratch3-glide-to-object]]]

**Порада:** Коли ти перетягуєш спрайт на Сцені, блоки Руху, які застосовують координати `x`{:class="block3motion"} та `y`{:class="block3motion"} оновлюються у меню блоків `Рух`{:class="block3motion"}. Нинішні координати `x`{:class="block3motion"} та `y`{:class="block3motion"} відображаються на панелі Спрайта.

### Обертання
Ти також можеш змінювати `напрям`{:class="block3motion"}, на який направлений спрайт. Це змінить напрямок, в якому буде рухатися спрайт, якщо ти використаєш блок `перемістити на`{:class="block3motion"}. Також можна змінювати обертання образу спрайта в залежності від налаштування `стиль обертання`{:class="block3motion"}.

Коли ти додаєш новий спрайт, він буде направлений праворуч (90 градусів). Ти можеш змінювати це на панелі спрайтів або за допомогою блоків коду.

```blocks3
turn right [15] degrees

turn left [15] degrees

point in direction [90] // Click on 90 and drag the arrow to change

point towards (mouse-pointer v)

(direction)

set rotation style [left-right v] // or all-around or none
```

[[[scratch3-sprite-direction]]]

[[[scratch3-left-right-direction]]]

--- collapse ---
---
title: Обертатися навколо
---

--- no-print ---

**Кажан обертається**: [Переглянути код](https://scratch.mit.edu/projects/435704980/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435704980/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Цей код змушує спрайт обертатися при натисканні на зелений прапорець:

```blocks3
when flag clicked
forever
turn right (1) degrees :: motion
```

У блоці `поворот на`{:class="block3motion"}, який має в собі цикл `завжди`{:class="block3control"}, зміни кількість градусів на `1` і твій спрайт почне обертатися.

**Порада:** Якщо ти не додаєш блок `перемістити на`{:class="block3motion"}, твій спрайт буде обертатися в тому положенні, в якому він і знаходиться.

--- /collapse ---

--- collapse ---
---
title: Рух по колу
---

--- no-print ---

**Орбіта Місяця**: [Переглянути код](https://scratch.mit.edu/projects/435701055/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435701055/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Цей код змушує спрайт літати по колу при натисканні на зелений прапорець:

```blocks3
when green flag clicked
forever
move (1) steps
turn right (1) degrees :: motion
```

Зміни значення у блоці `рухатись на`{:class="block3motion"} та у блоці `поворот на`{:class="block3motion"}, які вставлені в цикл `завжди`{:class="block3control"} на `1`, і твій спрайт буде рухатися по колу.

**Порада:** Якщо ти хочеш, щоб твій спрайт завжди починав рух з центру Сцени, ти можеш додати блок `перемістити в x:`{:class="block3motion"} `0` `y:`{:class="block3motion"} `0` перед блоком `завжди`{:class="block3control"}.

--- /collapse ---

### Відбивання

Блок `якщо на межі, відбити`{:class="block3motion"} дуже корисний, коли ти хочеш змусити спрайт відбиватися і залишатися на Сцені:

```blocks3
if on edge, bounce
```

Ось кілька способів, як можна змусити спрайт відбиватися:

--- collapse ---
---
title: Відбивання по сцені
---

--- no-print ---

**Дівчинка рухається по сцені**: [Переглянути код](https://scratch.mit.edu/projects/433535326/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433535326/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Цей код змушує спрайт відбиватись від лівого та правого країв Сцени. Тому що спрайт обертається горизонтально, здається, що він обертається, коли змінює свій напрямок, при натисканні на зелений прапорець:

```blocks3
when green flag clicked
point in direction (90)
set rotation style [left-right v]
forever
move (5) steps
if on edge, bounce
```

У цьому прикладі, блок `повернути в напрямку`{:class="block3motion"} автоматично направляє спрайт вправо на (`90` градусів), при натисканні на зелений прапорець. Якщо ти зміниш кількість градусів на `-90`, твій спрайт буде направлений ліворуч.

Додай блок `стиль обертання`{:class="block3motion"} та вибери у спливаючому меню `зліва-направо`{:class="block3motion"}, щоб твій спрайт не перевертався догори ногами, коли відбивається від краю Сцени.

**Порада:** Ти можеш перетягнути свій спрайт по Сцені, щоб розташувати його в потрібній тобі позиції за віссю Y (вгору-вниз).

--- /collapse ---

--- collapse ---
---
title: Відбивання по сцені вниз і вверх
---

--- no-print ---

**Дівчинка стрибає**: [Переглянути код](https://scratch.mit.edu/projects/433595822/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433595822/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Цей код змушує спрайт відбиватися вгору і вниз по сцені при натисканні на зелений прапорець:

```blocks3
when green flag clicked
point in direction (0)
set rotation style [don't rotate v]
forever
move (5) steps
if on edge, bounce
```

Зміни число градусів у блоці `повернути в напрямку`{:class="block3motion"} на `0`, щоб спрайт був направлений вгору.

Додай блок `стиль обертання`{:class="block3motion"} та вибери у спливаючому меню `не обертати`{:class="block3motion"}, щоб зупинити обертання спрайта, коли він відбивається.

**Порада:** Ти можеш перетягнути свій спрайт по Сцені, щоб розмістити його в потрібній тобі позиції x (ліворуч-праворуч).

--- /collapse ---

--- collapse ---
---
title: Відбивання від кута
---

--- no-print ---

**Футбольні відбивання**: [Переглянути код](https://scratch.mit.edu/projects/433536479/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433536479/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Цей код змушує спрайт випадковим чином обертатися, при натисканні на зелений прапорець:

```blocks3
when green flag clicked
point in direction (45)
set rotation style [all around v]
forever
move (5) steps
if on edge, bounce
```

Якщо твій спрайт переміщується зі швидкістю `45` градусів, ти побачиш, що він відбивається від краю Сцени з певним нахилом. Зміни число градусів у блоці `повернути в напрямку`{:class="block3motion"} на `45`, щоб твій спрайт відбивався на всі сторони.

Додай блок `стиль обертання`{:class="block3motion"} та вибери у спливаючому меню `навколо`{:class="block3motion"}, щоб твій спрайт обертався, коли буде відбиватися від краю Сцени.

--- /collapse ---

### Використання координат

Також ти можеш `змінити`{:class="block3motion"} та `задати`{:class="block3motion"} координати `x`{:class="block3motion"} та `y`{:class="block3motion"}, щоб отримати їх значення для використання в інших блоках:

[[[generic-scratch3-coordinates]]]

```blocks3 
change x by [10]

set x to [0]

change y by  [10]

set y to [0]

(x position)

(y position)
```

--- collapse ---
---
title: Я не бачу ніяких блоків Руху
---

Якщо ти вибираєш Сцену, то ти не побачиш жодних блоків `Рух`{:class="block3motion"}, тому що Сцена не може рухатися.

Клацни по спрайту на панелі Спрайт, а потім клацни по вкладці **Код**, щоб побачити блоки `Рух`{:class="block3motion"}.

--- /collapse ---

