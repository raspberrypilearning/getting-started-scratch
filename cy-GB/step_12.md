## Gweithredwyr

Mae'r blociau `Gweithredwyr`{:class="block3operators"} yn cael eu defnyddio i gymharu newidynnau a gwerthoedd, gwneud cyfrifiadau â rhifau, a gweithio gyda llinynnau (testun).

Mae'r blociau hecsagon 'Boole' yn cael eu defnyddio fel cyflyrau, ac maen nhw'n dychwelyd gwir neu anwir. Gellir defnyddio'r blociau yma mewn blociau `Control`{:class="block3control"} gyda mewnbwn hecsagonol.

Gweithredwyr cymhariaeth:

```blocks3
<[] > [50]>

<[] < [50]>

<[] = [50]>
```

**Awgrym:** Pan fyddi di'n defnyddio`=`{:class="block3operators"} gyda thestun galli di gymysgu llythrennau bach a mawr, felly mae `<`{:class="block3operators"} `YDY` `=`{:class="block3operators"} `ydy` `>`{:class="block3operators"} yn dychwelyd **gwir**.


Mae'r rhain yn weithrediadau mathemateg:

```blocks3
([] + [])

([] - [])

([] * [])

([] / [])
```

Galli di ddewis rhifau ar hap rhwng y rhif lleiaf a'r mwyaf (gan gynnwys y rhifau hynny).

```blocks3
(pick random [1] to [10]) // Rhif rhwng o 1 i 10
```

Mae'r gweithredwyr `a`{:class="block3operators"}, `neu`{:class="block3operators"}, a `nid`{:class="block3operators"} yn gallu cael eu defnyddio i gyfuno cyflyrau.

```blocks3
<<> and <>>

<<> or <>>

<not <> >
```

Mae blociau ar gyfer gweithio gyda llinynnau testun:

```blocks3
(join [apple ] [banana])

(letter [1] of [apple])

(length of [apple])

<[apple] contains [a]>
```

[[[scratch3-join-text]]]

Mae yna hefyd rhagor o weithredwyr mathemateg sy'n ddefnyddiol ar gyfer rhai prosiectau.
