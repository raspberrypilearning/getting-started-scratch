## Waarnemen

De blokken in het `Waarnemen`{:class="block3sensing"} blokkenmenu worden gebruikt om tekstinvoer van gebruikers te krijgen, voorwaarden te ontdekken en te rapporteren over waarden in je project.

Er zijn verschillende hexagonale `Waarnemen`{:class="block3sensing"}-blokken die je kunt gebruiken in `Besturen`{:class="block3control"}-blokken om beslissingen te nemen en te controleren wanneer blokken worden uitgevoerd.

Met het `raken`{:class="block3sensing"}-blok kun je waarnemen of de sprite die eigenaar is van het script de muisaanwijzer (waar je je vinger voor het laatst hebt aangeraakt op een tablet), de rand van het werkgebied of een andere sprite raakt:

```blocks3
<touching (mouse-pointer v) ?>

<touching (edge v) ?>

<touching (Sprite2 v) ?>
```

Er zijn blokken om waar te nemen of de sprite die eigenaar is van het script een andere kleur raakt (in het werkgebied of een andere sprite), of dat een kleur op deze sprite een andere kleur raakt.

```blocks3
<touching color (#c5a97b) ?>

<color (#c219ed) is touching (#62d1e0) ?>
```

Het `toets ingedrukt`{:class="block3sensing"} blok heeft opties voor cijfer-, letter- en pijltoetsen. Je hebt een toetsenbord nodig om hier waarden te kunnen invoeren. Het neemt waar of de toets momenteel wordt ingedrukt:

```blocks3
<key (space v) pressed?>
```

Het `muis ingedrukt`{:class="block3sensing"}-blok neemt waar of de muis momenteel wordt ingedrukt, of op het scherm wordt getikt of aangeraakt op een touchscreen:

```blocks3
<mouse down?>
```

De `vraag`{:class="block3sensing"} en `antwoord`{:class="block3sensing"} blokken worden gebruikt om tekstinvoer van de gebruiker te krijgen:

```blocks3
ask [Hoe heet jij] and wait

(answer) // de tekst die de gebruiker heeft getypt 
```

Het `vraag`{:class="block3sensing"}-blok werkt met een toetsenbord of met een virtueel schermtoetsenbord op een tablet.

Het `antwoord`{:class="block3sensing"}-blok is een blok dat een waarde terug geeft en dat ook als variabele kan worden gebruikt.

[[[scratch3-ask-answer-chat]]]

Het `Waarnemen`{:class="block3sensing"} blokkenmenu bevat ook verschillende blokken die kunnen worden gebruikt om waarden op te halen:

```blocks3
(distance to (mouse-pointer v))

(distance to (Sprite2 v))
```

Je kunt de huidige positie van de muisaanwijzer waarnemen (of de huidige of meest recente positie van je vinger op een tablet):

```blocks3
(mouse x)

(mouse y)
```

Je kunt het `volume`{:class="block3sensing"} van het geluid van de microfoon waarnemen. Een pop-upvenster vraagt de gebruiker om toestemming om de microfoon te gebruiken:

```blocks3
(loudness)
```

De `klok`{:class="block3sensing"} begint te tellen wanneer het project wordt geladen en kan worden teruggezet naar `0` met het `zet klok op 0`{:class="block3sensing"} blok:

```blocks3
(timer)

reset timer
```

Je hebt ook toegang tot meldingen voor het Speelveld en andere sprites:

```blocks3
([backdrop # v] of (_stage_ v))

([x position v] of (Sprite2 v))

([costume # v] of (Sprite2 v))
```

Er zijn meldingen gerelateerd aan de datum en tijd in de echte wereld, in je lokale tijdzone:

```blocks3
(current [year v]) // uur, minuut, ...

(days since 2000)
```

