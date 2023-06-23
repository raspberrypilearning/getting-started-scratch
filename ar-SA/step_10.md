## التحكم

كتل`التحكم`{:class="block3control"} تتحكم بالترتيب الذي تشتغل فيه الكتل, متضمنا القرارات (التعيين) و الحلقات ( التكرار).


كتلة `انتظر`{:class="block3control"} تأخر لعدد من الثواني قبل تشغيل كتلة التالية.

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

**نصيحة:** يمكنك إيقاف كتلة `إلى الأبد`{:class="block3events"} بضغط على زر قف أعلى المنصة, أو باستخدام كتل `قف`{:class="block3control"}.

هناك ثلاثة خيارات لكتلة `قف`{:class="block3events"}:

```blocks3
stop [all v] // stop all scripts in all sprites

stop [this script v]

stop [other scripts in sprite v]
```

الكتل `إذا...إذن`{:class="block3control"} و `إذا...إذن...آخر`{:class="block3control"} تستعمل لاتخاذ قرار حول أي كتلة كود سوف يتم تشغيلها تاليا. هذه تسمى أحيانا **تعيين**. كتلة `إذا...إذن`{:class="block3control"} تتحقق **شرط** سداسي الشكل و تشغل كتل الكود داخلا, إذا كان الشرط **صحيح**. لكتلة `إذا...إذن..آخر`{:class="block3control"} قسم إضافي لتشغيل كتل الكود داخلا, إذا كان الشرط **خطأ**.

```blocks3
if <> then

end

if <> then

else

end
```

[[[scratch3-if-then-else]]]

يمكنك إيجاد كتل سداسية الشكل لتستخدمها كشروط في قائمة الكتلتين `العاملين`{:class="block3operators"} و `الاستشعار`{:class="block3sensing"}.

كتلتي `انتظر حتى`{:class="block3control"} و `كرر حتى`{:class="block3control"} أيضا تستخدمان الشروط:

```blocks3
wait until <> // delay until the condition is true


repeat until <> // repeat the blocks inside until the condtion is true

end
```

**المستنسخ** هو نسخة من الكائن, له زي, نص و صوت المحمول من قبل الكائن المستنسخ منه وقت النسخ. هناك عدد من الكتل التي يمكن استخدامها لاستنساخ الكائنات.

بكتلة` خلق مستنسخ من [نفسي v]`{:class="block3control"}, يمكن لمخلوق خلق مستنسخا من نفسه أو من مخلوق آخر في المشروع.

```blocks3
create clone of [myself v] // clones the sprite that runs this block


create clone of [Butterfly 1 v] // clones another sprite in the project
```

قبعة الكتلة `عندما أبدأ كمستنسخ`{:class="block3control"} تستخدم لإطلاق نص جديد بمجرد خلق المستنسخ. المستنسخ سيتواجد في المشروع حتى تستخدم قبعة كتلة `احذف هذا المستنسخ`{:class="block3control"}.

استعمل قبعة كتلة `عند بدئي كمستنسخ`{:class="block3control"} ثم إضافة كتلة ` اخلق مستنسخا من [نفسي v]`{:class="block3control"} في النص أسفله تعني أنه بإمكان المستنسخين خلق مستنسخين اخرين.

```blocks3
when I start as a clone // the script that runs when the clone is created


delete this clone // stops the clone's scripts and deletes it
```

هناك عدد أقصى للمستنسخين الذين يمكن أن يملكهم مخلوق في أي مرحلة, في وقت كتابة هذا هو `300`.

--- collapse ---
---
title: مستنسخو المستنسخين
---

**المستنسخون**: [انظر في الداخل](https://scratch.mit.edu/projects/567544298/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567544298/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /collapse ---

