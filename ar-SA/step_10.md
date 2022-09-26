## التحكم

مجموعات`التحكم`{:class="block3control"} تتحكم الترتيب الذي تشتغل فيه المجموعات, متضمنا القرارات (التعيين) و الحلقات ( التكرر).مجموعةمجموعة


مجموعة `انتظر`{:class="block3control"} تأخر لعدد من الثواني قبل تشغيل المجموعة التالية.

```blocks3
wait (1) seconds// delay for 1 second

wait (0.1) seconds// delay for one tenth of a second
```

الحلقات تتحكم كم مرة يتكرر الكود داخلها.

```blocks3
repeat (4) // run the blocks inside four time

end
```

```blocks3
forever // run the blocks inside until stopped

end
```

[[[scratch3-forever-condition]]]

**نصيحة:** يمكنك إيقاف المجموعة `إلى الأبد`{:class="block3events"} بضغط زر قف أعلى المنصة, أو باستخدام مجموعة `قف`{:class="block3control"}.

هناك ثلاثة خيارات لمجموعة `قف`{:class="block3events"}:

```blocks3
stop [all v] // stop all scripts in all sprites

stop [this script v]

stop [other scripts in sprite v]
```

المجموعات `if...then `{:class="block3control"} و `if...then...else `{:class="block3control"} تستعمل لاتخاذ قرار حول أي مجاميع كودات سوف يتم تشغيلها. هذه تسمى أحيانا **تعيين**. مجموعة `if...then`{:class="block3control"} تتحقق **شرط** سداسي الشكل و تشغل مجاميع الكود داخلها, إذا كان الشرط **صحيح**. The `if...then..else`{:class="block3control"} block has an additional section to run the code blocks inside, if the condition is **false**.

```blocks3
if <> then

end

if <> then

else

end
```

[[[scratch3-if-then-else]]]

You can find hexagonal-shaped blocks to use as conditions in the `Operators`{:class="block3operators"} and `Sensing`{:class="block3sensing"} blocks menus.

The `wait until`{:class="block3control"} and `repeat until`{:class="block3control"} blocks also use conditions:

```blocks3
wait until <> // delay until the condition is true


repeat until <> // repeat the blocks inside until the condtion is true

end
```

A **clone** is a copy of a sprite, it has the costumes, scripts and sounds held by the sprite it was cloned from at the time of cloning. There are a number of blocks that can be used to clone sprites.

With the `create clone of [myself v]`{:class="block3control"} block, a sprite can create a clone of itself or of another sprite in the project.

```blocks3
create clone of [myself v] // clones the sprite that runs this block


create clone of [Butterfly 1 v] // clones another sprite in the project
```

The `when I start as a clone`{:class="block3control"} hat block is used to trigger a new script once the clone has been created. The clone will exist in the project until the `delete this clone`{:class="block3control"} cap block is used.

Using the `when I start as a clone`{:class="block3control"} hat block then including the `create clone of [myself v]`{:class="block3control"} block in the script underneath means it is also possible for clones to create other clones.

```blocks3
when I start as a clone // the script that runs when the clone is created


delete this clone // stops the clone's scripts and deletes it
```

There is a maximum number of clones a sprite can have at any point, at the time of writing this is `300`.

--- collapse ---
---
title: Clones of clones
---

**Clones**: [See inside](https://scratch.mit.edu/projects/567544298/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567544298/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /collapse ---

