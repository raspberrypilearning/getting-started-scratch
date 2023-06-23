## Змінні

`Змінна`{:class="block3variables"} - це спосіб зберігання чисел та/або тексту.

Ти можеш створювати власні змінні та вибирати, чи показувати їх на Сцені:

[[[generic-scratch3-add-variable]]]

Тобі варто подумати над тим, чи треба задати початкове значення, коли створюєш змінну:

[[[scratch3-create-set-variable]]]

Ти можеш змінити назву змінної, якщо передумаєш:

--- collapse ---
---
title: Перейменування змінної
---

Іноді ти можеш придумати кращу назву для змінної.

Ти можеш дати змінній нову назву: перейди в меню блоків `Змінні`{:class="block3variables"}, клацни правою кнопкою миші (або на планшеті торкнись і утримуй) на `моя змінна`{:class="block3variables"}, та вибери **Перейменувати змінну**.

![Вибір 'Перейменувати змінну' в меню.](images/rename-variable.png)

Таким чином буде змінено назву змінної в усіх блоках, в яких ти її використовуєш.

--- /collapse ---

**Порада:** Переконайся, що ти знаєш різницю між `надати`{:class="block3variables"} та `змінити на`{:class="block3variables"}. `надати`{:class="block3variables"} замінить значення, яке зберігається у змінній. `змінити на`{:class="block3variables"} змінить значення числа змінної на обрану тобою величину, `змінити на`{:class="block3variables"}`1` додасть до змінної одиницю. `змінити на`{:class="block3variables"}`-1` відніме від змінної одиницю.


**Порада:** Змінні на Сцені завжди відображаються на першому плані відносно всіх спрайтів. Якщо у тебе є рухомий спрайт, то він буде ходити під будь-якими змінними на Сцені.

Для регулювання значення у змінній можна використовувати слайдер.

[[[scratch3-slider-variable]]]

Більше ідей для використання змінних:

[[[generic-scratch3-high-score]]]

[[[scratch3-join-text]]]

[[[scratch3-set-variable-with-button]]]

[[[scratch3-change-variable-in-loop]]]


--- collapse ---
---
title: Регулювання графічних ефектів за допомогою слайдера змінної
---

Ось кілька прикладів того, як можна використовувати слайдер змінної:


Цей приклад змінює графічний ефект `привид`{:class="block3looks"}, щоб можна було бачити наскрізь веселку.

**Прозора веселка**: [Переглянути код](https://scratch.mit.edu/projects/451544795/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/451544795/?autostart=false" frameborder="0"></iframe>
</div>

Ти можеш використовувати змінну `transparent`{:class="block3variables"}, щоб контролювати ефект на спрайті `привід`{:class="block3looks"}, який розміщений на `передній`{:class="block3looks"} план, і використати його, щоб показати або приховати спрайти на задніх планах.

```blocks3
when flag clicked
go to [front v] layer
```

```blocks3
when flag clicked
forever
set [ghost v] effect to (transparent)
```

Спробуй використати так само інші графічні ефекти, наприклад, `яскравість`{:class="block3looks"} або `колір`{:class="block3looks"}.

--- /collapse ---

--- collapse ---
---
title: Регулювання швидкості руху за допомогою змінної
---

**Сонечка на стіні**: [Переглянути код](https://scratch.mit.edu/projects/451545341/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/451545341/?autostart=false" frameborder="0"></iframe>
</div>

Використовуй змінну `speed`{:class="block3variables"}, яка вставлена у блок `перемістити на`{:class="block3motion"}:

```blocks3
when flag clicked
forever
move (speed) steps
if on edge, bounce
```
Встанови мінімальне і максимальне значення, використовуючи діапазон слайдера, відповідно до твого проєкту.

--- /collapse ---

--- collapse ---
---
title: Регулювання швидкості повороту за допомогою змінної
---

**Космічний пес**: [Переглянути код](https://scratch.mit.edu/projects/451543041/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/451543041/?autostart=false" frameborder="0"></iframe>
</div>

Використовуй змінну `angle`{:class="block3variables"}, яка вставлена в блок `поворот на право`{:class="block3motion"}:

```blocks3
when flag clicked
forever
turn right (angle) degrees
```

--- /collapse ---

--- collapse ---
---
title: Зміна затримки в блоці чекати
---

**Танець скелета**: [Переглянути код](https://scratch.mit.edu/projects/451536565/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/451536565/?autostart=false" frameborder="0"></iframe>
</div>

Використовуй змінну `delay`{:class="block3variables"}, яка вставлена в блок `чекати`{:class="block3control"}:

```blocks3
when flag clicked
forever
wait (delay) seconds
next costume
```

Затримка більш ніж на одну секунду - це досить тривалий час. Якщо встановити діапазон слайдера на десяткове число, тоді можна змінювати значення на 100-ту долю секунди.

Діапазон від `0.00` до `1.00` дозволяє вибрати затримку між `0` секундами(без затримки) та `1` секундою.

![Зміна діапазону слайдера від 0.00 до 1.00.](images/decimal-delay.png)

Змінюй числа, щоб отримати мінімальне і максимальне значення, яке ти хочеш, щоб інші користувачі могли використовувати у твоєму проєкті.

--- /collapse ---

--- collapse ---
---
title: Зміна звукових ефектів
---

**Налаштування барабана**: [Переглянути код](https://scratch.mit.edu/projects/451547017/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/451547017/?autostart=false" frameborder="0"></iframe>
</div>

Використовуй `змінну`{:class="block3variables"}, яка знаходиться у блоці `встановити ефект висота в`{:class="block3sound"}. Якщо ти збільшуєш висоту звуку, то ноти стають вищими, а звук прискорюється.

```blocks3
when flag clicked
forever
set [pitch v] effect to (beat) :: sound
```

Запуск звук в окремому циклі `завжди`{:class="block3control"}, щоб висота тону змінювалася негайно, а не чекати, поки звук відтвориться заново:

```blocks3
when flag clicked
forever
play sound [Dance Head Nod v] until done
```

Ти також можеш використовувати `змінну`{:class="block3variables"}, щоб змінити гучність і ефект панорамування (нахилу).

--- /collapse ---



