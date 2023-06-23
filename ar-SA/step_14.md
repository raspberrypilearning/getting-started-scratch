## كتلي (التعليمات البرمجية الخاصة بالمستخدم)

`لبناتي`{: class = "block3myblocks"} تسمح لك بإنشاء كتل جديدة للكائن. تقوم بتسمية الكتلة البرمجية ثم `تحدد`{: class = "block3myblocks"} ما تفعله الكتلة البرمجية الجديدة باستخدام كتل Scratch الأخرى. يمكنك استخدام الكتلة البرمجية الجديدة في أي جزء من المشروع على الكائن الذي يمتلك كتلة من لبناتي.

يعرّف هذا المثال كتلة برمجية من لبناتي `talk`{: class = "block3myblocks"} و التي تعمل على تغيير المظهر الخارجي للكائن:

**تغريد البطريق**: [انظر من الداخل](https://scratch.mit.edu/projects/567554899/editor){: target = "_ blank"}

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

يمكنك استخدام `My Blocks`{: class = "block3myblocks"} لتنظيم **** الشفرة البرمجية لمشروعك. من الأسهل تجميع كل الكتل البرمجية التي تجعل كائنًا يتحدث ثم استخدم كتلة واحدة `talk`{: class = "block3myblocks"} عندما تريد أن يتحدث الكائن.

إذا قررت أنك تريد تغيير الطريقة التي يتحدث بها الكائن ، فعليك تغيير الشفرة البرمجية في مكان واحد فقط.

### لبناتي مع المدخلات

يمكنك أيضًا إضافة **مدخلات ** إلى `لبناتي`{: class = "block3myblocks"} بحيث تستخدم القيم التي تقدمها لها المستخدم عند استخدام الكتلة.

**محادثات البطريق**: [انظر من الداخل](https://scratch.mit.edu/projects/567538874/editor){: target = "_ blank"}

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
العنوان: استخدم لبناتي لتنظيم التعليمات البرمجية
---
إن أبسط طريقة لاستخدام `لبناتي`{: class = "block3myblocks"} هي المساعدة في تنظيم التعليمات البرمجية الخاصة بك. اليك مثال بسيط.

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

`لبناتي`{: class = "block3myblocks"} تشبه "الإجراءات" أو "الوظائف" أو "الدوال" في لغات البرمجة الأخرى.
