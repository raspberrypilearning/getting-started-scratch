## Czujniki

Bloki w menu `Czujniki`{:class="block3sensing"} służą do wprowadzania tekstu przez użytkownika, wykrywania warunków i raportowania wartości w projekcie.

Istnieje kilka sześciokątnych bloków sekcji `Czujniki`{:class="block3sensing"}, których można użyć w blokach `Kontrola`{:class="block3control"} do podejmowania decyzji i sterowania uruchamianiem bloków.

Blok `dotyka`{:class="block3sensing"} ma opcje wykrywania, czy duszek będący właścicielem skryptu dotyka wskaźnika myszy (w miejscu, w którym ostatnio dotykałeś palcem na tablecie), krawędzi Sceny, czy innego duszka:

```blocks3
<touching (mouse-pointer v) ?>

<touching (edge v) ?>

<touching (Sprite2 v) ?>
```

Są bloki pozwalające wykryć, czy duszek będący właścicielem skryptu dotyka innego koloru (na Scenie lub innego duszka), czy też kolor na tym duszku dotyka innego koloru.

```blocks3
<touching color (#c5a97b) ?>

<color (#c219ed) is touching (#62d1e0) ?>
```

Blok `klawisz naciśnięty?`blok {:class="block3sensing"} ma opcje dla cyfr, liter i strzałek. Aby móc wprowadzać klawisze, potrzebujesz klawiatury. Ten blok wykrywa, czy klawisz jest aktualnie wciśnięty:

```blocks3
<key (space v) pressed?>
```

Blok `kliknięto myszką?`{:class="block3sensing"} wykrywa, czy przycisk myszy jest aktualnie wciśnięty albo czy ekran zostaje stuknięty lub dotykany na ekranie dotykowym:

```blocks3
<mouse down?>
```

Bloki `zapytaj`{:class="block3sensing"} i `odpowiedź`{:class="block3sensing"} służą do wprowadzania tekstu przez użytkownika:

```blocks3
ask [What's your name] and wait

(answer) // the text the the user typed 
```

Blok `zapytaj`{:class="block3sensing"} działa z klawiaturą lub wirtualną klawiaturą ekranową na tablecie.

Blok `odpowiedź`{:class="block3sensing"} jest blokiem raportującym, który zgłasza wartość i może być używany jako zmienna.

[[[scratch3-ask-answer-chat]]]

Bloki z grupy `Czujniki`{:class="block3sensing"} zawierają również kilka bloków raportujących, których można użyć do uzyskania wartości:

```blocks3
(distance to (mouse-pointer v))

(distance to (Sprite2 v))
```

Możesz wykryć aktualną pozycję wskaźnika myszy (lub aktualną lub ostatnią pozycję palca na tablecie):

```blocks3
(mouse x)

(mouse y)
```

Możesz wykryć `głośność`{:class="block3sensing"} dźwięku z mikrofonu. Wyskakujące okienko poprosi użytkownika o pozwolenie na korzystanie z mikrofonu:

```blocks3
(loudness)
```

Blok `stoper`{:class="block3sensing"} rozpoczyna odliczanie po załadowaniu projektu i można go ustawić z powrotem na `0` z użyciem bloku `resetuj stoper`{:class="block3sensing"}:

```blocks3
(timer)

reset timer
```

Możesz także sięgnąć do bloków raportujących dla Sceny i innych duszków:

```blocks3
([backdrop # v] of (_stage_ v))

([x position v] of (Sprite2 v))

([costume # v] of (Sprite2 v))
```

Istnieją bloki raportujące powiązane z datą i godziną w realnym świecie, w Twojej strefie czasowej:

```blocks3
(current [year v]) // hour, minute, ...

(days since 2000)
```

