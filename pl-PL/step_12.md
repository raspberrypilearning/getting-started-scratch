## Wyrażenia

Bloki z menu `Wyrażenia`{:class="block3operators"} służą do porównywania zmiennych i wartości, wykonywania obliczeń i pracy z napisami (tekstem).

Sześciokątne bloki „Boole'a” (czytaj: Bula) są używane jako warunki i zwracają prawdę albo fałsz. Bloki te mogą być używane w blokach z menu `Kontrola`{:class="block3control"} z wejściem sześciokątnym.

Operatory porównania:

```blocks3
<[] > [50]>

<[] < [50]>

<[] = [50]>
```

**Wskazówka:** Gdy użyjesz `=`{:class="block3operators"} z tekstem, możesz mieszać małe i duże litery, więc `<`{:class="block3operators"} `TAK` `=`{:class ="block3operators"} `tak` `>`{:class="block3operators"} zwraca wartość **prawda**.


Są to operacje matematyczne:

```blocks3
([] + [])

([] - [])

([] * [])

([] / [])
```

Możesz wylosować liczby spomiędzy podanej najmniejszej i największej liczby (włącznie z tymi liczbami).

```blocks3
(pick random [1] to [10]) // A number from 1 to 10
```

Operatory `i`{:class="block3operators"}, `lub`{:class="block3operators"} oraz `nie`{:class="block3operators"} mogą być używane do łączenia warunków.

```blocks3
<<> and <>>

<<> or <>>

<not <> >
```

Istnieją bloki do pracy z napisami (ciągami tekstowymi):

```blocks3
(join [apple ] [banana])

(letter [1] of [apple])

(length of [apple])

<[apple] contains [a]>
```

[[[scratch3-join-text]]]

Jest też więcej operatorów matematycznych, które są przydatne w niektórych projektach.
