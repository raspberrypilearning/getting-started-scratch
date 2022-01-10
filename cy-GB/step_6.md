## Symudiad

Mae blociau `Symudiad`{:class="block3motion"} yn caniatáu i ti symud dy gorlun o amgylch y Llwyfan.

### Symudiad

Y bloc `symudiad`{:class="block3motion"} yw'r ffordd symlaf i ddechrau gyda symud corlun:

```blocks3
move [10] steps
```

Galli di ddewis `mynd i`{:class="block3motion"} neu `llithro i`{:class="block3motion"} bwyntydd y llygoden, safle ar hap ar y Llwyfan (neu dy fys ar dabled), neu gorlun arall:

```blocks3
go to (random position v)

glide [1] secs to (random position v)
```

Galli di hefyd ddewis `mynd i`{:class="block3motion"} neu `llithro i`{:class="block3motion"} safle a roddir gan gyfesurynnau `x`{:class="block3motion"} a `y`{:class="block3motion"} ar y Llwyfan.

```blocks3
go to x: [0] y: [0] 

glide [1] secs to x: [0] y: [0]
```

[[[scratch3-glide-to-object]]]

**Awgrym:** Pan fyddi di'n llusgo corlun ar i'r llwyfan, mae'r blociau symud sy'n defnyddio cyfesurynnau `x`{:class="block3motion"} a `y`{:class="block3motion"} yn diweddaru yn y ddewislen blociau `Symudiad`{:class="block3motion"}. Mae'r cyfesurynnau `x`{:class="block3motion"} a `y`{:class="block3motion"} presennol yn ymddangos yn y cwarel Corlun.

### Cylchdroi
Galli di hefyd newid y `cyfeiriad`{:class="block3motion"} mae corlun yn pwyntio tuag ato. Mae hyn yn newid y cyfeiriad bydd y corlun yn symud iddo os wyt ti'n defnyddio bloc `symudiad`{:class="block3motion"}. Gall hyn hefyd newid y ffordd mae gwisg y corlun yn cylchdroi gan ddibynu ar osodiad y `steil-cylchdroi`{:class="block3motion"}.

Pan fyddi di'n ychwanegu corlun, bydd yn wynebu'r dde (90 gradd). Galli di newid hwn yn cwarel y Corlun neu ddefnyddio blociau cod.

```blocks3
turn right [15] degrees

turn left [15] degrees

point in direction [90] // Clicia ar 90 a llusgo'r saeth i newid

point towards (mouse-pointer v)

(direction)

set rotation style [left-right v] // neu o amgylch neu beidio troi
```

[[[scratch3-sprite-direction]]]

[[[scratch3-left-right-direction]]]

--- collapse ---
---
title: Troelli o gwmpas
---

--- no-print ---

**Ystlum sy'n troelli**: [Gweld tu mewn](https://scratch.mit.edu/projects/435704980/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435704980/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Mae'r cod hwn yn gwneud i gorlun droelli pan gaiff y fflag werdd ei chlicio:

```blocks3
when flag clicked
forever
turn right (1) degrees :: motion
```

Mewn bloc `troi`{:class="block3motion"} o fewn dolen `am byth`{:class="block3control"} newidia nifer y graddau i `1` a bydd dy gorlun yn dechrau troelli.

**Awgrym:** Os nad wyt ti'n ychwanegu bloc `symud`{:class="block3motion"}, bydd dy gorlun yn parhau i droelli yn y safle mae ynddo.

--- /collapse ---

--- collapse ---
---
title: Symud mewn cylch
---

--- no-print ---

**Orbit lleuad**: [Gweld tu mewn](https://scratch.mit.edu/projects/435701055/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435701055/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Mae'r cod yma yn gwneud i gorlun hedfan mewn cylch pan fydd y faner werdd wedi'i chlicio:

```blocks3
when green flag clicked
forever
move (1) steps
turn right (1) degrees :: motion
```

Newidia'r gwerthoedd mewn bloc `symud`{:class="block3motion"} a bloc `troi`{:class="block3motion"} o fewn dolen `am byth`{:class="block3control"} i `1` a bydd dy gorlun yn symud mewn cylch mawr.

**Awgrym:** Os wyt ti am i dy gorlun ddechrau yng nghanol y Llwyfan bob amser, galli di ychwanegu bloc `mynd i x:`{:class="block3motion"} `0` `y:`{:class="block3motion"} `0` cyn y bloc `am byth`{:class="block3control"}.

--- /collapse ---

### Bowndio

Mae'r bloc `os ar yr ymyl, bowndio`{:class="block3motion"} yn arbennig o ddefnyddiol os wyt ti am wneud i dy gorlun fowndio o gwmpas ac aros ar y Llwyfan:

```blocks3
if on edge, bounce
```

Cymer olwg ar rai o'r ffyrdd galli di gael dy gorlun i fowndio o gwmpas:

--- collapse ---
---
title: Bowndio ar draws y Llwyfan
---

--- no-print ---

**Merch yn symud ar draws y Llwyfan**: [Gweld tu mewn](https://scratch.mit.edu/projects/433535326/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433535326/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Mae'r cod hwn yn gwneud i gorlun fowndio ar ymylon chwith a dde'r Llwyfan. Oherwydd bod y corlun yn cylchdroi yn llorweddol, bydd yn edrych fel petai'n fflipio wrth newid ei gyfeiriad pan gaiff y faner werdd ei chlicio:

```blocks3
when green flag clicked
point in direction (90)
set rotation style [left-right v]
forever
move (5) steps
if on edge, bounce
```

Yn yr enghraifft hon, mae'r bloc `pwyntio i gyfeiriad`{:class="block3motion"} yn pwyntio'r corlun i'r dde (`90` degrees) yn awtomatig pan gaiff y fflag werdd ei chlicio. Os byddi di'n newid nifer y graddau i `-90`, bydd dy gorlun yn pwyntio i'r chwith.

Ychwanega floc `gosod steil cylchdroi`{:class="block3motion"} a dewis `chwith-dde`{:class="block3motion"} yn y gwymplen, fel na fydd dy gorlun di'n fflipio wyneb i waered pan fydd yn bowndio ar ymyl y Llwyfan.

**Awgrym:** Galli di lusgo dy gorlun ar y Llwyfan i'w symud i'r safle y (i fyny-i lawr) rwyt ti ei eisiau.

--- /collapse ---

--- collapse ---
---
title: Bowndio i fyny ac i lawr y Llwyfan
---

--- no-print ---

**Merch yn neidio**: [Gweld tu mewn](https://scratch.mit.edu/projects/433595822/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433595822/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Mae'r cod yma yn gwneud i gorlun neidio i fyny ac i lawr ar y Llwyfan pan gaiff y faner werdd ei chlicio:

```blocks3
when green flag clicked
point in direction (0)
set rotation style [don't rotate v]
forever
move (5) steps
if on edge, bounce
```

Newidia nifer y graddau yn y bloc `pwyntio i gyfeiriad`{:class="block3motion"} i `0` i wneud i'r corlun bwyntio i fyny.

Ychwanega floc `gosod steil cylchdroi`{:class="block3motion"} a dewis `peidio cylchdroi`{:class="block3motion"} yn y gwymplen i stopio dy gorlun rhag cylchdroi, hyd yn oed pan fydd yn bowndio.

**Awgrym:** Galli di lusgo dy gorlun o amgylch y Llwyfan i'w symud i'r safle x (chwith-dde) rwyt ti ei eisiau.

--- /collapse ---

--- collapse ---
---
title: Bowndio ar ongl
---

--- no-print ---

**Bowndio pêl droed**: [Gweld tu mewn](https://scratch.mit.edu/projects/433536479/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433536479/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Mae'r cod yma yn gwneud i gorlun gylchdroi ar hap pan gaiff y faner werdd ei chlicio:

```blocks3
when green flag clicked
point in direction (45)
set rotation style [all around v]
forever
move (5) steps
if on edge, bounce
```

Os ydy dy gorlun yn symud ar ongl o `45` gradd, fe weli di ei fod yn edrych fel petai'n bowndio ar ymyl y Llwyfan ar ongl. Newidia nifer y graddau yn y bloc `pwyntio i gyfeiriad`{:class="block3motion"} i `45` i wneud i dy gorlun fowndio o gwmpas.

Ychwanega floc `gosod steil cylchdroi`{:class="block3motion"} a dewis `o amgylch`{:class="block3motion"} yn y gwymplen, fel bod dy gorlun yn troi pan fydd yn bowndio ar ymyl y Llwyfan.

--- /collapse ---

### Defnyddio cyfesurynnau

Galli di hefyd `newid`{:class="block3motion"} a `gosod`{:class="block3motion"} y cyfesurynnau `x`{:class="block3motion"} a `y`{:class="block3motion"} a chael eu gwerthoedd i'w defnyddio mewn blociau eraill:

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
title: Alla i ddim gweld unrhyw flociau Symudiad
---

Os wyt ti wedi dewis y Llwyfan yna fyddi di ddim yn gweld unrhyw flociau `Symudiad`{:class="block3motion"}, oherwydd dydy'r Llwyfan ddim yn gallu symud.

Clicia ar gorlun yng nghwarel y Corlun ac wedyn clicio ar y tab **Cod** i weld y blociau `Symudiad`{:class="block3motion"}.

--- /collapse ---

