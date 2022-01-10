## Synhwyro

Mae'r blociau yn y ddewislen `Synhwyro`{:class="block3sensing"} yn cael eu defnyddio i gael mewnbwn testun gan ddefnyddwyr, canfod cyflyrau, ac adrodd ar werthoedd yn dy brosiect.

Mae sawl bloc hecsagon `Synhwyro`{:class="block3sensing"} y galli di eu defnyddio mewn blociau `Rheoli`{:class="block3control"} i wneud penderfyniadau ac i reoli pryd bydd blociau'n cael eu rhedeg.

Mae gan y bloc `cyffwrdd`{:class="block3sensing"} opsiynau ar gyfer canfod a ydy'r corlun sydd biau'r sgript yn cyffwrdd pwyntydd y llygoden (neu'r lle diwethaf i dy fys gyffwrdd ar dabled), ymyl y llwyfan, neu gorlun arall:

```blocks3
<touching (mouse-pointer v) ?>

<touching (edge v) ?>

<touching (Sprite2 v) ?>
```

Mae blociau ar gyfer canfod a ydy'r corlun sydd biau'r sgript yn cyffwrdd â lliw arall (ar y Llwyfan neu gorlun arall), neu a ydy lliw ar y corlun hwn yn cyffwrdd â lliw arall.

```blocks3
<touching color (#c5a97b) ?>

<color (#c219ed) is touching (#62d1e0) ?>
```

Mae gan y bloc `bysell wedi'i phwyso?`{:class="block3sensing"} opsiynau ar gyfer bysellau rhif, llythyren, a saeth. Mae angen bysellfwrdd arnat ti i allu defnyddio bysellau. Mae'n canfod a yw'r fysell yn cael ei phwyso ar hyn o bryd:

```blocks3
<key (space v) pressed?>
```

Mae'r bloc `llygoden i lawr`{:class="block3sensing"} yn canfod a ydy'r llygoden yn cael ei bwyso ar hyn o bryd, neu a ydy'r sgrin yn cael ei daro neu ei gyffwrdd ar sgrin cyffwrdd:

```blocks3
<mouse down?>
```

Mae'r blociau `gofyn`{:class="block3sensing"} ac `ateb`{:class="block3sensing"} yn cael eu defnyddio i gael mewnbwn testun gan y defnyddiwr:

```blocks3
ask [What's your name] and wait

(answer) // the text the the user typed 
```

Mae'r bloc `gofyn`{:class="block3sensing"} yn gweithio gyda bysellfwrdd neu gyda bysellfwrdd rhithwir ar y sgrin ar dabled.

Mae'r bloc `ateb`{:class="block3sensing"} yn floc adroddwr sy'n adrodd gwerth ac mae modd ei ddefnyddio fel newidyn.

[[[scratch3-ask-answer-chat]]]

Mae'r ddewislen blociau `Synhwyro`{:class="block3sensing"} yn cynnwys sawl bloc adroddwr y mae modd eu defnyddio i gael gafael ar werthoedd:

```blocks3
(distance to (mouse-pointer v))

(distance to (Sprite2 v))
```

Galli di ganfod lleoliad presennol pwyntydd y llygoden (neu safle presennol neu ddiweddaraf dy fys ar dabled):

```blocks3
(mouse x)

(mouse y)
```

Galli di ganfod `cryfder sain`{:class="block3sensing"} o'r meicroffon. Bydd ffenestr naid yn gofyn i'r defnyddiwr am ganiatâd i ddefnyddio'r meicroffon:

```blocks3
(loudness)
```

Mae'r `amserydd`{:class="block3sensing"} yn dechrau cyfrif pa fydd y prosiect yn llwytho, ac mae modd ei osod yn ôl i `0` gydag `ailosod amserydd`{:class="block3sensing"}:

```blocks3
(timer)

reset timer
```

Galli di hefyd gael mynediad at adroddwyr ar gyfer y Llwyfan a chorluniau eraill:

```blocks3
([backdrop # v] of (_stage_ v))

([x position v] of (Sprite2 v))

([costume # v] of (Sprite2 v))
```

Mae yna adroddwyr sy'n gysylltiedig â'r dyddiad a'r amser yn y byd go iawn, yn dy gylch amser lleol:

```blocks3
(current [year v]) // hour, minute, ...

(days since 2000)
```

