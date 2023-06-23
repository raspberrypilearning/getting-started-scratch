## Вигляд

Блоки `Вигляд`{:class="block3looks"} керують появою спрайта на Сцені.

Спрайти можуть спілкуватися між собою за допомогою блоків `Вигляд`{:class="block3looks"}, використовуючи мовну бульбашку `говорити`{:class="block3looks"}, або бульбашку думок `подумати`{:class="block3looks"}, або через їхні `графічні ефекти`{:class="block3looks"}.

### Говорити та подумати

```blocks3
say () for () seconds

say ()

think () for () seconds

think ()
```

--- collapse ---
---
title: Використання мовної бульбашки для спілкування
---

Щоб спілкуватися, спрайти можуть `говорити`{:class="block3looks"} та `подумати`{:class="block3looks"}.

Блоки `говорити () () сек`{:class="block3looks"} та `подумати () () сек`{:class="block3looks"} використовуються для того, щоб сказати або подумати щось протягом певного часу.

```blocks3
when this sprite clicked
say [Hello!] for [2] seconds // hide speech after 2 seconds
```

Якщо натиснути, спрайт покаже мовну бульбашку на дві секунди.

**Космічна розмова**: [Переглянути код](https://scratch.mit.edu/projects/485673032/editor){:target="_blank"}

Клацни по спрайтах, щоб побачити, як вони спілкуються мовою та думками.

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/485673032/?autostart=false" frameborder="0"></iframe>
</div>

Блоки `говорити ()`{:class="block3looks"} та `подумати ()`{:class="block3looks"} використовуються для того, щоб щось говорити або думати, поки не з'явиться інше повідомлення або порожній блок, який замінить`говорити ()`{:class="block3looks"} або `подумати ()`{:class="block3looks"}.

--- /collapse ---

### Розмір

Встанови або зміни `розмір`{:class="block3looks"} твоїх спрайтів.

```blocks3
change size by ()

set size to () %

(size)
```

--- collapse ---
---
title: Встанови розмір спрайта
---

Коли ти додаєш спрайт до проєкту, його розмір встановлено на `100` відсотків. Це може бути занадто великим або занадто малим для твого проєкту.

Ти можеш задати розмір спрайта за допомогою коду. Для цього використовуй блок `задати розмір`{:class="block3looks"}:

```blocks3
set size to (50) %
```

Якщо ти встановиш розмір спрайта на `50` відсотків, то він буде вдвічі меншим у висоту і вдвічі меншим у ширину. Якщо ти встановиш розмір спрайта на `200` відсотків, то він буде вдвічі вищим і вдвічі ширшим.

Щоб задати розмір спрайта при запуску проєкту, додай блок `задати розмір`{:class="block3looks"} під блоком `коли зелений прапорець натиснуто`{:class="block3events"}:

```blocks3
when green flag clicked
set size to (50) %
```

Також ти можеш швидко встановити розмір спрайта у параметрі **Розмір** на панелі Спрайт, який знаходиться під Сценою:

![Поле параметру Розмір на панелі Спрайт виділено.](images/spriteSize.png){:width="400px"}

--- /collapse ---

### Графічні ефекти

Встановлення або зміна різних візуальних ефектів, таких як колір, роздуття, закручування, пікселями, мозаїка, яскравість та привид.

```blocks3
change [color v] effect by ()

set [color v] effect to ()

clear graphic effects
```

[[[scratch3-graphic-effects]]]

### Образи

Щоб створити ефект анімації зі своїми спрайтами, ти можеш змінювати їх образи.

```blocks3
switch costume to ( v)

next costume

(costume [number v])
```

[[[scratch3-change-costumes-to-show-mood]]]

--- collapse ---
---
title: Створення анімації за допомогою зміни вигляду
---

**Серцебиття**: [Переглянути код](https://scratch.mit.edu/projects/435725413/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/435725413/?autostart=false" frameborder="0"></iframe>
</div>

Ти можеш використовувати блоки `задати розмір`{:class="block3looks"} або `змінити розмір на`{:class="block3looks"}, щоб створити ефект, що пульсує, наприклад серцебиття.

**Порада:** Блок `задати розмір`{:class="block3looks"} встановлює розмір на певне значення, тоді як блок `змінити розмір на`{:class="block3looks"} змінює значення в порівнянні з тим, яке було раніше, наприклад `змінити розмір на`{:class="block3looks"} `10` збільшує значення розміру на 10.

```blocks3
when green flag clicked
set size to (160) %
forever
change size by (40)
wait (0.2) seconds
change size by (20)
wait (0.2) seconds
change size by (-20)
wait (0.2) seconds
change size by (-40)
wait (0.2) seconds
end
```

Цей код використовує ряд блоків `змінити розмір на`{:class="block3looks"} та `чекати`{:class="block3control"}, щоб змусити серце збільшуватися і зменшуватися. Спробуй створити свій власний спрайт, який пульсує.

Ти також можеш використовувати блок `змінити графічний ефект на`{:class="block3looks"}, щоб створити спрайт, який буде продовжувати змінювати свій зовнішній вигляд.

```blocks3
when green flag clicked
change [ghost v] effect by (75)
wait (1) seconds
change [ghost v] effect by (-75)
```

**Порада:** Якщо ти використовуєш код, який спочатку змінює графічний ефект, а потім повертає його назад, не забудь використати блок `чекати`{:class="block3control"} між блоками `змінити графічний ефект на`{:class="block3looks"}, інакше це станеться так швидко, що ти й не помітиш!

Ти можеш використати в будь-який момент блок `очистити графічні ефекти`{:class="block3looks"}, щоб скасувати дію ефектів:

```blocks3
clear graphic effects
```

--- /collapse ---

--- collapse ---
---
title: Клацни, щоб змінити, а потім повернути назад
---

Ти можеш додавати дії, які змінюють спрайт, а потім поверти все назад, наприклад, роздутись, чекати, а потім стиснутись.

**Роздуття м'яча при натисканні**: [Переглянути код](https://scratch.mit.edu/projects/435723273/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435723273/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

Цей код буде роздувати спрайт - застосуй ефект `роздуття `{:class="block3looks"} на 0,5 секунд, а потім поверни спрайт до початкового вигляду:

```blocks3
when this sprite clicked
set size to (110)
set [fisheye v] effect to (50)
wait (0.5) seconds
set [fisheye v] effect to (0)
set size to (100)
```

--- /collapse ---

[[[scratch3-animate-movement-costumes]]]

### Тло

Також можна використовувати код, щоб змінити тло.

```blocks3
switch backdrop to ( v)

next backdrop

(backdrop [number v])
```

[[[scratch3-changing-backdrops-pages-levels]]]

### Видимість

Блоки `показати`{:class="block3looks"} та `сховати`{:class="block3looks"} керують видимість спрайта.

```blocks3
show 

hide
```

[[[scratch3-show-hide-sprites-backdrops]]]

### Плани

Щоб змінювати розташування спрайтів відносно один одного, ти можеш використовувати плани.

```blocks3
go to [front v] layer

go [forward v] () layers
```

[[[scratch3-positioning-with-layers]]]

--- collapse ---
---
title: Розташування спрайтів у багатьох планах
---

**Крізь вікно з деревом**: [Переглянути код](https://scratch.mit.edu/projects/454188775/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/454188775/?autostart=false" frameborder="0"></iframe>
</div>

На приклад, спрайт **Window frame** відображається спереду, а спрайт **Sun** відображається ззаду. Спрайти **Avery Walking** та **Tree** знаходяться кожен на своїх планах, між спрайтом **Window frame** та спрайтом **Sun**.

Використовуй блок `перемістити назад на`{:class="block3looks"} `1` `шар`{:class="block3looks"}, щоб перемістити спрайт на один план позаду спрайта, який знаходиться спереду:

``` blocks3
when green flag clicked
go to [front v] layer
+go [backward v] (1) layers
```

Зміни значення в полі блока `перемістити назад`{:class="block3looks"} `1` `шар`{:class="block3looks"} для кожного спрайта, залежно від того, як ти хочеш його розташувати стосовно до інших спрайтів:

``` blocks3
when green flag clicked
go to [front v] layer
+go [backward v] (2) layers
```

--- /collapse ---

