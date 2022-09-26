## الحركة.

كتل `الحركة`{: class = "block3motion"} تسمح لك تحريك الكائن حول المنصة.

### الحركة

كتلة `تحرك`{:class="block3motion"} هي أبسط طريق لتبدأ بتحريك كائن:

```blocks3
move [10] steps
```

يمكنك ` الذهاب إلى`{:class="block3motion"} أو `انزلق خلال`{:class="block3motion"} مؤشر الفأرة, موقع عشوائي على المنصة (أو إصبعك على اللوحة), أو كائن آخر:

```blocks3
go to (random position v)

glide [1] secs to (random position v)
```

يمكنك أيضا `الذهاب إلى`{:class="block3motion"} أو `الزحلقة إلى`{:class="block3motion"} موقع معطى بإحداثيات `x`{:class="block3motion"} و `y`{:class="block3motion"} على المنصة.

```blocks3
go to x: [0] y: [0] 

glide [1] secs to x: [0] y: [0]
```

[[[scratch3-glide-to-object]]]

**نصيحة:** عند سحبك كائنا على المنصة, كتل الحركة التي تستعمل تحديث إحداثيات `x`{:class="block3motion"} و `y`{:class="block3motion"} في قائمة كتل `الحركة`{:class="block3motion"}. إحداثيات `x`{:class="block3motion"} and `y`{:class="block3motion"} الحالية تظهر على قائمة الكائن.

### دوران
يمكنك أيضًا تغيير الاتجاه ``{: class = "block3motion"} الذي يشير إليه الكائن. يغير هذا الاتجاه الذي سينتقل إليه الكائن إذا استخدمت كتلة `move`{: class = "block3motion"}. يمكن أيضا أن تغير دوران زي الكائن إعتمادا على خيار `نمط الدوران`{:class="block3motion"}.

عند إضافة كائن ، سيواجه اليمين (90 درجة). يمكنك تغيير هذا في قائمة الكائن أو باستخدام كتل الكود.

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
العنوان: تدور حول
---

--- no-print ---

**العصا الدوارة**:[انظر داخلا](https://scratch.mit.edu/projects/435704980/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435704980/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

هذا الكود يجعل الكائن يدور عند النقر على العلم الأخضر:

```blocks3
when flag clicked
forever
turn right (1) degrees :: motion
```

في كتلة `منعطف`{: class = "block3motion"} داخل حلقة `إلى الأبد`{: class = "block3control"} ، قم بتغيير عدد الدرجات إلى `1` وسيظهر الكائن الخاص بك يدور.

**نصيحة:** إذا لم تضف كتلة `تحرك`{:class="block3motion"}, كائنك سيدور في مكانه.

--- /collapse ---

--- collapse ---
---
العنوان: التحرك في دائرة
---

--- no-print ---

**مدار القمر**:[أنظر داخلا](https://scratch.mit.edu/projects/435701055/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435701055/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

هذا الكود يجعل الكائن يطير في دائرة عند النقر على العلم الأخضر:

```blocks3
when green flag clicked
forever
move (1) steps
turn right (1) degrees :: motion
```

غير القيم في كتلة `تحرك`{:class="block3motion"} و كتلة ` استدر`{:class="block3motion"} في حلقة `كرر باستمرار`{:class="block3control"} إلى `1` و كائنك سيظهر حركة في دائرة كبيرة.

**نصيحة:** إذا أردت كائنك أن يبدأ دائما من مركز المنصة, يمكنك إضافة كتلة `إذهب إلى x`{:class="block3motion"} `0` `y:`{:class="block3motion"} `0` قبل كتلة `كرر باستمرار`{:class="block3control"}.

--- /collapse ---

### الإرتداد

كتلة `إرتد إذا كنت عند الحافة`{:class="block3motion"} جد مفيدة عند حاجتك لصنع كائن يرتد و يبقى على المنصة:

```blocks3
if on edge, bounce
```

شاهد بعض الطرق التي يمكنك من خلالها جعل كائنك يرتد:

--- collapse ---
---
العنوان: ترتد عبر المنصة
---

--- no-print ---

**فتاة تتحرك عبر المنصة**:[أنظر داخلا](https://scratch.mit.edu/projects/433535326/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433535326/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

هذا الكود يجعل الكائن يرتد على حواف المنصة اليمنى و اليسرى. لأن الكائن يدور أفقيا, يظهر متشقلبا عند تغييره إتجاهه عند ضغط العلم الأخضر:

```blocks3
when green flag clicked
point in direction (90)
set rotation style [left-right v]
forever
move (5) steps
if on edge, bounce
```

في هذا المثال ، النقطة `في الاتجاه`{: class = "block3motion"} تقوم الكتلة تلقائيًا بتوجيه الكائن إلى اليمين (90`` درجات) عند النقر فوق العلم الأخضر. إذا قمت بتغيير عدد الدرجات إلى 0-90 `، فإن`الكائن الخاص بك سوف يشير إلى اليسار.

أضف كتلة `اجعل نمط الدوران`{:class="block3motion"} و عين` يسار-يمين`{:class="block3motion"} في القائمة النازلة, إذا كائنك لن يتشقلب رأسا على عقب عند إرتداده على جانب المنصة.

**نصيحة:** يمكنك سحب كائنك على المنصة لتحريكه إلى الموضع y (أعلى-أسفل) الذي تريده.

--- /collapse ---

--- collapse ---
---
العنوان: ترتد صعودا وهبوطا على المنصة.
---

--- no-print ---

** فتاة تقفز**:[أنظر داخلا](https://scratch.mit.edu/projects/433595822/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433595822/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

هذا الكود يجعل الكائن يرتد أعلى و أسفل المنصة عند النقر على العلم الأخضر:

```blocks3
when green flag clicked
point in direction (0)
set rotation style [don't rotate v]
forever
move (5) steps
if on edge, bounce
```

غير عدد الدرجات في كتلة `اتجه نحو الإتجاه`{:class="block3motion"} إلى `0` لجعل الكائن يواجه الأعلى.

أضف كتلة `اجعل نمط الدوران`{:class="block3motion"} و عين ` لا دوران`{:class="block3motion"} في القائمة النازلة لإيقاف دوران كائنك, حتى عند ارتداده.

**نصيحة:** يمكنك سحب كائنك حول المنصة لتحريكه إلى الموضع x (يسار-يمين) الذي تريده.

--- /collapse ---

--- collapse ---
---
العنوان: ترتد بزاوية
---

--- no-print ---

**كرة قدم الإرتداد**:[أنظر داخلا](https://scratch.mit.edu/projects/433536479/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433536479/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

هذا الكود يجعل الكائن يظهر يدور عشوائيا عند النقر على العلم الأخضر:

```blocks3
when green flag clicked
point in direction (45)
set rotation style [all around v]
forever
move (5) steps
if on edge, bounce
```

إذا تحرك كائنك عند `45`درجة, ستجد أنه يظهر يرتد على حافة المنصة بزاوية. غير عدد الدرجات في كتلة `اتجه نحو الإتجاه`{:class="block3motion"} إلى `45` لجعل كائنك يرتد في كل الأرجاء.

أضف كتلة `اجعل نمط الدوران`{:class="block3motion"} و عين `في جميع الإتجاهات`{:class="block3motion"} في القائمة المنسدلة, إذا كائنك سيدور عند ارتداده على حافة المنصة.

--- /collapse ---

### إستعمال الإحداثيات

يمكنك أيضا `تغيير`{:class="block3motion"} و `وضع`{:class="block3motion"} الإحداثيتين `x`{:class="block3motion"} و `y`{:class="block3motion"} و إيجاد قيمتيهما لاستعمالهما في كتل أخرى:

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
العنوان: لا يمكنني رؤية أي كتل متحركة
---

إذا حددت المنصة ، فلن ترى أي كتل `حركة`{: class = "block3motion"} ، لأن المنصة لا يمكن أن تتحرك.

انقر على كائن في لائحة الكائنات ثم انقر على تبويب **الكود** لرؤية كتل `الحركة`{:class="block3motion"}.

--- /collapse ---

