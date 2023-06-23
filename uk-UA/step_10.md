## Керування

Блоки `Керування`{:class="block3control"} контролюють порядок виконання блоків, включаючи прийняття рішень (вибір) та цикли (повторення).


Блок `чекати`{:class="block3control"} створює затримку певну кількість секунд перед запуском наступного блоку.

```blocks3
wait (1) seconds// delay for 1 second

wait (0.1) seconds// delay for one tenth of a second
```

Цикли керують тим, скільки разів буде виконуватися код, який знаходиться всередині них.

```blocks3
repeat (4) // run the blocks inside four time

end
```

```blocks3
forever // run the blocks inside until stopped

end
```

[[[scratch3-forever-condition]]]

**Порада:** Ти можеш зупинити блок `завжди`{:class="block3events"} натиснувши кнопку Зупинити, яка знаходиться над Сценою, або за допомогою блоків `зупинити`{:class="block3control"}.

Існує три опції для блоку `зупинити`{:class="block3events"}:

```blocks3
stop [all v] // stop all scripts in all sprites

stop [this script v]

stop [other scripts in sprite v]
```

Блоки `якщо...то`{:class="block3control"} та `якщо...то...інакше`{:class="block3control"} приймають рішення про те, які блоки коду запускати наступними. Інколи це називається **вибір**. Блок `якщо...то`{:class="block3control"} перевіряє шестигранну форму **умова** і запускає блоки коду, які знаходяться всередині, якщо виконується умова **true**. Блок `якщо...то...інакше`{:class="block3control"} має додаткову секцію для виконання блоків коду, якщо виконується умова **false**.

```blocks3
if <> then

end

if <> then

else

end
```

[[[scratch3-if-then-else]]]

Ти можеш знайти блоки шестигранної форми та використовувати їх як умови у меню блоках`Оператори`{:class="block3operators"} та `Датчики`{:class="block3sensing"}.

Блоки `чекати поки`{:class="block3control"} та `повторити до`{:class="block3control"} також використовують умови:

```blocks3
wait until <> // delay until the condition is true


repeat until <> // repeat the blocks inside until the condtion is true

end
```

**Клон** це копія спрайта, який має образи, скрипти та звуки, якими володів спрайт, з якого він був створений на момент клонування. Є декілька блоків, які можна використовувати для клонування спрайтів.

За допомогою блока `створити клон з [мене v]`{:class="block3control"}, спрайт може створити клон самого себе або іншого спрайта в проєкті.

```blocks3
create clone of [myself v] // clones the sprite that runs this block


create clone of [Butterfly 1 v] // clones another sprite in the project
```

Блок з шапкою `коли я починаю як клон`{:class="block3control"} використовується для запуску нового скрипту одразу після створення клону. Клон буде існувати в проєкті до тих пір, поки не буде використано блок `вилучити цей клон`{:class="block3control"}.

Використовуючи блок з шапкою `коли я починаю як клон`{:class="block3control"}, який містить в собі блок `створити клон з [мене v]`{:class="block3control"} означає, що клони також зможуть створювати інші клони.

```blocks3
when I start as a clone // the script that runs when the clone is created


delete this clone // stops the clone's scripts and deletes it
```

Максимальна кількість клонів, яку може мати спрайт одночасно, на момент написання статті становить `300`.

--- collapse ---
---
title: Клони клонів
---

**Клони**: [Переглянути код](https://scratch.mit.edu/projects/567544298/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567544298/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /collapse ---

