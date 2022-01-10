## Functies

De `Functies`{:class="block3operators"} blokken worden gebruikt om variabelen en waarden te vergelijken, berekeningen met getallen uit te voeren en met strings (tekst) te werken.

De zeshoekige 'Boolean'-blokken worden gebruikt als voorwaarden en geven een waar of onwaar melding terug. Deze blokken kunnen worden gebruikt in `Besturen`{:class="block3control"} blokken met een zeshoekige ingang.

Vergelijkingen:

```blocks3
<[] > [50]>

<[] < [50]>

<[] = [50]>
```

**Tip:** Als je de `=`{:class="block3operators"} vergelijking met tekst gebruikt, kun je hoofdletters en kleine letters door elkaar gebruiken, dus `<`{:class="block3operators"} `YES` `=`{:class ="block3operators"} `yes` `>`{:class="block3operators"} geeft **waar**.


Er zijn wiskundige bewerkingen:

```blocks3
([] + [])

([] - [])

([] * [])

([] / [])
```

Je kunt willekeurige getallen kiezen tussen het kleinste en grootste getal (inclusief die getallen).

```blocks3
(pick random [1] to [10]) // A number from 1 to 10
```

De `en`{:class="block3operators"}, `of`{:class="block3operators"} en `niet`{:class="block3operators"} vergelijkingen kunnen worden gebruikt om voorwaarden te combineren.

```blocks3
<<> and <>>

<<> or <>>

<not <> >
```

Er zijn blokken om met tekst (strings) te werken:

```blocks3
(join [apple ] [banana])

(letter [1] of [apple])

(length of [apple])

<[apple] contains [a]>
```

[[[scratch3-join-text]]]

Er zijn ook meer wiskundige vergelijkingen die nuttig zijn voor sommige projecten.
