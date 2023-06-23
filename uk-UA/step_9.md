## Події

Блоки в меню `Події`{:class="block3events"} контролюють запуск скриптів.

**Блоки з шапкою** запускають блоки під ними, коли відбувається певна подія. Вони мають заокруглену верхівку, як шапка, тому жоден блок не може бути розташований вище за них.

Ти можеш використовувати:

```blocks3

when flag clicked // run blocks when the green flag above the Stage is clicked

when this sprite clicked // run the blocks when the sprite for this script is clicked

when stage clicked // run the blocks when the stage is clicked

```

**Порада:** Блок `коли сцену натиснуто`{:class="block3events"} доступний тільки тоді, коли ти працюєш в області Коду для Сцени.

Якщо ти користуєшся комп'ютером з клавіатурою, ти можеш використовувати блоки `коли клавішу натиснуто`{:class="block3events"}:

```blocks3
when [space v] key pressed // change to number, letter or arrow keys
```

Також можна використовувати блок `коли тло зміниться на`{:class="block3events"}, щоб запустити скрипт під час зміни тла.

[[[scratch3-changing-backdrops-pages-levels]]]

[[[scratch3-show-hide-sprites-backdrops]]]


Блок `коли >`{:class="block3events"} має дві версії:

```blocks3
when [loudness v] > (10) // run blocks when the microphone detects sound

when [timer v] > (10) // run blocks when the timer reaches 10 seconds
```

[[[scratch3-time-delay]]]


Два останні блоки в меню `Події`{:class="block3events"} це блоки `оповістити`{:class="block3events"}. Ти можеш використовувати блок `коли я отримую (повідомлення v)`{:class="block3events"}, щоб запустити скрипт при запуску будь-якого спрайта, який збігається з блоком `коли я отримую (повідомлення v)`{:class="block3events"}.

[[[generic-scratch3-broadcast-message]]]

