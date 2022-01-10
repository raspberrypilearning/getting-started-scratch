## Rheoli

Mae blociau `Rheoli`{:class="block3control"} yn rheoli'r drefn y mae blociau'n rhedeg ynddi, gan gynnwys penderfyniadau (dewis) a dolenni (ailadrodd).


Mae'r bloc `aros`{:class="block3control"} yn oedi am nifer o eiliadau cyn rhedeg y bloc nesaf.

```blocks3
wait (1) seconds// oedi am 1 eiliad

wait (0.1) seconds// oedi am un rhan o ddeg o eiliad
```

Mae dolenni'n rheoli faint o amser mae'r cod y tu mewn iddyn nhw yn rhedeg.

```blocks3
repeat (4) // rhedeg y blociau sydd tu mewn bedair gwaith

end
```

```blocks3
forever // rhedeg y blociau sydd tu mewn nes eu stopio

end
```

[[[scratch3-forever-condition]]]

**Awgrym:** Galli di stopio bloc `am byth`{:class="block3events"} drwy glicio'r botwm Aros uwchben y Llwyfan, neu drwy ddefnyddio'r blociau `aros`{:class="block3control"}.

Mae yna dri opsiwn ar gyfer y bloc `aros`{:class="block3events"}:

```blocks3
stop [all v] // stopio pob sgript ym mhob corlun

stop [this script v]

stop [other scripts in sprite v]
```

Mae'r blociau `os...yna`{:class="block3control"} ac `os...yna...fel arall`{:class="block3control"} yn cael eu defnyddio i wneud penderfyniadau o ran pa flociau cod i'w rhedeg nesaf. Weithiau mae hyn yn cael ei alw'n **ddewis**. Mae'r bloc `os...yna`{:class="block3control"} yn gwirio **cyflwr** siâp hecsagon ac yn rhedeg y blociau cod tu mewn, os ydy'r cyflwr yn **wir**. Mae gan y bloc `os...yna...fel arall`{:class="block3control"} adran ychwanegol i redeg blociau cod ynddi, os ydy'r cyflwr yn **anghywir**.

```blocks3
if <> then

end

if <> then

else

end
```

[[[scratch3-if-then-else]]]

Galli di ddod o hyd i flociau siâp hecsagon i'w defnyddio fel cyflyrau yn y ddewslenni `Gweithredwyr`{:class="block3operators"} a `Synhwyro`{:class="block3sensing"}.

Mae'r blociau `aros hyd at`{:class="block3control"} ac `ailadrodd hyd at`{:class="block3control"} hefyd yn defnyddio cyflyrau:

```blocks3
wait until <> // oedi nes bod y cyflwr yn wir


repeat until <> // ailadrodd y blociau sydd tu mewn nes bod y cyflwr yn wir

end
```

Mae **clôn** yn gopi o gorlun, mae ganddo'r gwisgoedd, y sgriptiau a'r seiniau oedd yn berchen ar y corlun cafodd ei glonio ohono ar amser y broses clonio. Mae yna nifer o flociau y gellir eu defnyddio i glonio corluniau.

Gyda'r bloc `creu clôn o [fi fy hun v]`{:class="block3control"}, mae corlun yn gallu creu clôn ohono'i hun neu o gorlun arall yn y prosiect.

```blocks3
create clone of [myself v] // clonio'r corlun sy'n rhedeg y bloc hwn


create clone of [Butterfly 1 v] // clonio corlun arall yn y prosiect
```

Mae'r bloc het `pan rwy'n dechrau fel clôn`{:class="block3control"} yn cael ei ddefnyddio i sbarduno sgript newydd ar ôl i'r clôn gael ei chreu. Bydd y clôn yn bodoli yn y prosiect nes bydd y bloc cap `dileu'r clôn hwn`{:class="block3control"} yn cael ei ddefnyddio.

Mae defnyddio'r bloc het `pan rwy'n dechrau fel clôn`{:class="block3control"} ac yna cynnwys y bloc `creu clôn o [fi fy hun v]`{:class="block3control"} yn y sgript oddi tano yn golygu ei fod hefyd yn bosib i glonau greu clonau eraill.

```blocks3
when I start as a clone // y sgript sy'n rhedeg pan fydd y clôn yn cael ei greu


delete this clone // yn stopio sgriptiau'r clôn ac yn ei ddileu
```

Mae uchafswm o glonau y gall corlun eu cael ar unrhyw adeg, ar adeg ysgrifennu'r canllaw yma yr uchafswm ydy `300`.

--- collapse ---
---
title: Clonau o glonau
---

**Clonau**: [Gweld tu mewn](https://scratch.mit.edu/projects/567544298/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567544298/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /collapse ---

