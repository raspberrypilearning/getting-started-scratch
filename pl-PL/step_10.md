## Kontrola

Bloki `Kontrola`{:class="block3control"} sterują kolejnością wykonywania bloków, w tym decyzje (wybór) i pętle (powtarzanie).


Blok `czekaj`{:class="block3control"} opóźnia wykonanie następnego bloku o podaną liczbę sekund.

```blocks3
wait (1) seconds// delay for 1 second

wait (0.1) seconds// delay for one tenth of a second
```

Pętle kontrolują, ile razy wykonywany jest w nich kod.

```blocks3
repeat (4) // run the blocks inside four time

end
```

```blocks3
forever // run the blocks inside until stopped

end
```

[[[scratch3-forever-condition]]]

**Wskazówka:** Możesz zatrzymać blok `zawsze`{:class="block3events"}, klikając przycisk Zatrzymaj nad Sceną lub używając bloków `zatrzymaj`{:class="block3control"}.

Istnieją trzy opcje dla bloku `zatrzymaj`{:class="block3events"}:

```blocks3
stop [all v] // stop all scripts in all sprites

stop [this script v]

stop [other scripts in sprite v]
```

Bloki `jeżeli...to`{:class="block3control"} i `jeżeli...to...w przeciwnym razie`{:class="block3control"} służą do podejmowania decyzji o tym, które bloki kodu mają zostać uruchomione w następnej kolejności. Jest to czasami nazywane **wyborem**. Blok `jeżeli...to`{:class="block3control"} sprawdza **warunek** sześciokąta i uruchamia bloki kodu wewnątrz, jeśli warunek jest **prawdziwy**(gdy jest spełniony). Blok `jeżeli...to...w przeciwnym razie`{:class="block3control"} ma dodatkową sekcję do uruchamiania bloków kodu wewnątrz, jeśli warunek to **fałsz**(gdy nie jest spełniony).

```blocks3
if <> then

end

if <> then

else

end
```

[[[scratch3-if-then-else]]]

Możesz znaleźć sześciokątne bloki, które będą używane jako warunki w menu bloków `Wyrażenia`{:class="block3operators"} i `Czujniki`{:class="block3sensing"}.

Bloki `czekaj aż`{:class="block3control"} i `powtarzaj aż`{:class="block3control"} również korzystają z warunków:

```blocks3
wait until <> // delay until the condition is true


repeat until <> // repeat the blocks inside until the condtion is true

end
```

**Klon** jest kopią duszka, posiada te same kostiumy, skrypty i dźwięki co duszek, z którego został sklonowany w momencie, kiedy nastąpiło klonowanie. Istnieje szereg bloków, których można użyć do klonowania duszków.

Za pomocą bloku `utwórz klona z [siebie v]`{:class="block3control"}, duszek może utworzyć klona z siebie samego lub z innego duszka w projekcie.

```blocks3
create clone of [myself v] // clones the sprite that runs this block


create clone of [Butterfly 1 v] // clones another sprite in the project
```

Blok kapelusz `gdy zaczynam jako klon`{:class="block3control"} jest używany do wystartowania nowego skryptu po utworzeniu klona. Klon będzie istniał w projekcie, dopóki nie zostanie użyty blok `usuń tego klona`{:class="block3control"}.

Użycie bloku kapelusza `gdy zaczynam jako klon`{:class="block3control"}, a następnie dołączanie pod nim bloku `utwórz klona z [siebie v]`{:class="block3control"} oznacza, że jest również możliwe tworzenie kolejnego klona z istniejącego klona.

```blocks3
when I start as a clone // the script that runs when the clone is created


delete this clone // stops the clone's scripts and deletes it
```

Istnieje maksymalna liczba klonów, jaką duszek może mieć w dowolnym momencie i w chwili pisania tego tekstu jest to `300`.

--- collapse ---
---
title: Klony klonów
---

**Klony**: [Zajrzyj do środka](https://scratch.mit.edu/projects/567544298/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567544298/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /collapse ---

