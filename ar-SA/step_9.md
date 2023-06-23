## الأحداث

الكتل البرمجية الموجودة في قائمة `الاحداث`{:class="block3events"} تتحكم في متى تبدأ الكائنات.

**مجموعة الكتل بشكل القبعة** تنفذ مجموعة الكتل البرمجية الموجودة اسفلها عند بدء حدث معين. هي مدورة من الأعلى، مثل القبعة، لذلك لا يمكن أن نضع الكتل فوقها.

يمكنك استخدام:

```blocks3

when flag clicked // run blocks when the green flag above the Stage is clicked

when this sprite clicked // run the blocks when the sprite for this script is clicked

when stage clicked // run the blocks when the stage is clicked

```

**نصيحة:** كتلة `عند نقر المنصة`{:class="block3events"} تكون متوفرة فقط عندما تعمل مع المقاطع البرمجية الخاصة بالمنصة.

إذا كنت تستخدم جهاز كمبيوتر ولوحة مفاتيح، فيمكنك استخدام `عند ضغط مفتاح`{:class="block3events"}:

```blocks3
when [space v] key pressed // change to number, letter or arrow keys
```

يمكنك ايضا استخدام كتلة `عندما تتبدل الخلفية الى`{:class="block3events"} لبدء النص البرمجي عندما تتغير الخلفية.

[[[scratch3-changing-backdrops-pages-levels]]]

[[[scratch3-show-hide-sprites-backdrops]]]


كتلة `عندما >` {:class="block3events"} لها نسختان:

```blocks3
when [loudness v] > (10) // run blocks when the microphone detects sound

when [timer v] > (10) // run blocks when the timer reaches 10 seconds
```

[[[scratch3-time-delay]]]


الكتلتين الاخيرتين في قائمة `الاحداث`{:class="block3events"} هما مجموعة `بث`:class="block3events"}. يمكن استخدام `عندما استلم (رسالة ١)`{:class="block3events"} لبدء النص البرمجي عندما يشتغل اي مقطع برمجي مطابق للرسالة في كتلة `بث (رسالة ١)`{:class="block3events"}.

[[[generic-scratch3-broadcast-message]]]

