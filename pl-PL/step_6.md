## Ruch

Bloki `Ruch`{:class="block3motion"} umożliwiają przesuwanie duszka po Scenie.

### Przesuwanie

Blok `przesuń o`{:class="block3motion"} to najprostszy sposób na rozpoczęcie przenoszenia duszka:

```blocks3
move [10] steps
```

Możesz użyć `idź do`{:class="block3motion"} lub `leć do`{:class="block3motion"} wskaźnika myszy, losowej pozycji na Scenie (lub palca na tablecie) lub innego duszka:

```blocks3
go to (random position v)

glide [1] secs to (random position v)
```

Możesz także użyć `idź do`{:class="block3motion"} lub `leć do`{:class="block3motion"} pozycji określonej przez współrzędne `x`{:class="block3motion"} i `y`{:class ="block3motion"} na Scenie.

```blocks3
go to x: [0] y: [0] 

glide [1] secs to x: [0] y: [0]
```

[[[scratch3-glide-to-object]]]

**Wskazówka:** Kiedy przeciągasz duszka na Scenę, bloki ruchu, które używają współrzędnych `x`{:class="block3motion"} i `y`{:class="block3motion"}, są aktualizowane w menu bloków `Ruch`{: class="block3motion"}. Aktualne współrzędne `x`{:class="block3motion"} i `y`{:class="block3motion"} są wyświetlane w panelu Sprite.

### Obrót
Możesz także zmienić `kierunek`{:class="block3motion"}, na który wskazuje duszek. To zmienia kierunek, w którym duszek będzie się poruszał kiedy użyjesz bloku `ruch`{:class="block3motion"}. Można w ten sposób również zmienić rotację kostiumu duszka w zależności od ustawienia `styl obrotu`{:class="block3motion"}.

Gdy dodasz nowego duszka, będzie on skierowany w prawo (90 stopni). Możesz to zmienić w Panelu duszków lub za pomocą bloków kodu.

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
title: Zakręć się
---

--- no-print ---

**Wirujący nietoperz**: [Zajrzyj do środka](https://scratch.mit.edu/projects/435704980/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435704980/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Ten kod powoduje obrót duszka po kliknięciu zielonej flagi:

```blocks3
po kliknięciu flagi
zawsze
obrót w prawo (1) stopnie :: ruch
```

W bloku `obróć`{:class="block3motion"} wewnątrz pętli `zawsze`{:class="block3control"}, zmień liczbę stopni na `1`, a twój duszek będzie się kręcił.

**Wskazówka:** Jeśli nie dodasz bloku `przesuń o`{:class="block3motion"}, twój duszek obróci się w miejscu, w którym się znajduje.

--- /collapse ---

--- collapse ---
---
title: Poruszaj się w kręgu
---

--- no-print ---

**Orbita Księżyca**: [Zajrzyj do środka](https://scratch.mit.edu/projects/435701055/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435701055/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Ten kod powoduje, że duszek będzie kręcił się w kółko po kliknięciu zielonej flagi:

```blocks3
po kliknięciu zielonej flagi
zawsze
ruch (1) kroki
obrót w prawo (1) stopnie :: ruch
```

Zmień wartości w bloku `przesuń o`{:class="block3motion"} i w bloku `obróć`{:class="block3motion"} w pętli `zawsze`{:class="block3control"} na `1`, a twój duszek pojawi się, aby poruszać się w dużym kręgu.

**Wskazówka:** Jeśli chcesz, aby Twój duszek zawsze ruszał ze środka Sceny, możesz dodać blok `idź do x:`{:class="block3motion"} `0` `y:`{:class="block3motion"} "} `0` przed blokiem `zawsze`{:class="block3control"}.

--- /collapse ---

### Odbijanie się

Blok `jeśli na brzegu, odbij się`{:class="block3motion"} jest naprawdę przydatny, gdy chcesz aby duszek odbijał się od krawędzi i pozostał na Scenie:

```blocks3
if on edge, bounce
```

Sprawdź kilka sposobów na to, aby Twój duszek się odbijał:

--- collapse ---
---
title: Odbijaj się na brzegach Sceny
---

--- no-print ---

**Dziewczynka poruszająca się na Scenie**: [Zajrzyj do środka](https://scratch.mit.edu/projects/433535326/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433535326/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Ten kod powoduje, że duszek odbija się od lewej i prawej krawędzi Sceny. Ponieważ duszek obraca się w poziomie, wygląda jakby się odwracał, gdy zmienia kierunek po kliknięciu zielonej flagi:

```blocks3
when green flag clicked
point in direction (90)
set rotation style [left-right v]
forever
move (5) steps
if on edge, bounce
```

W tym przykładzie blok`ustaw kierunek na`{:class="block3motion"} automatycznie kieruje duszka w prawo (`90` stopni) po kliknięciu zielonej flagi. Jeśli zmienisz liczbę stopni na `-90`, twój duszek zwróci się w lewo.

Dodaj blok `ustaw styl obrotu na`{:class="block3motion"} i wybierz `lewo-prawo`{:class="block3motion"} z rozwijanego menu, aby twój duszek nie odwrócił się do góry nogami podczas odbijania na skraju Sceny.

**Wskazówka:** Możesz przeciągnąć duszka na Scenie, aby przenieść go do żądanej pozycji y (góra-dół).

--- /collapse ---

--- collapse ---
---
title: Odbijaj się od góry i dołu Sceny
---

--- no-print ---

**Skacząca dziewczyna**: [Zajrzyj do środka](https://scratch.mit.edu/projects/433595822/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433595822/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Ten kod powoduje, że duszek odbija się na górze i dole Sceny po kliknięciu zielonej flagi:

```blocks3
when green flag clicked
point in direction (0)
set rotation style [don't rotate v]
forever
move (5) steps
if on edge, bounce
```

Zmień liczbę stopni w bloku `ustaw kierunek na`{:class="block3motion"} na `0` aby duszek skierował się w górę.

Dodaj blok `ustaw styl obrotu na`{:class="block3motion"} i wybierz `nie obracaj`{:class="block3motion"} z menu rozwijanego, aby zatrzymać obracanie duszka, nawet gdy się odbija.

**Wskazówka:** Możesz przeciągnąć duszka po Scenie, aby przenieść go do żądanej pozycji x (lewo-prawo).

--- /collapse ---

--- collapse ---
---
title: Odbijaj się pod kątem
---

--- no-print ---

**Odbijanie piłki nożnej**: [Zajrzyj do środka](https://scratch.mit.edu/projects/433536479/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433536479/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Ten kod sprawia, że duszek obraca się losowo po kliknięciu zielonej flagi:

```blocks3
when green flag clicked
point in direction (45)
set rotation style [all around v]
forever
move (5) steps
if on edge, bounce
```

Jeśli twój duszek porusza się pod kątem `45` stopni, zauważysz że odbija się od krawędzi Sceny pod pewnym kątem. Zmień liczbę stopni w bloku `ustaw kierunek na`{:class="block3motion"} na `45`, aby Twój duszek odbijał się dookoła.

Dodaj blok `ustaw styl obrotu na`{:class="block3motion"} i wybierz `dookoła`{:class="block3motion"} z rozwijanego menu, aby Twój duszek obrócił się, gdy odbije się od krawędzi Sceny.

--- /collapse ---

### Korzystanie ze współrzędnych

Możesz także użyć `zmień`{:class="block3motion"} i `ustaw`{:class="block3motion"} `x`{:class="block3motion"} i `y`{:class="block3motion"} i odczytać wartości współrzędnych aby je wykorzystać w innych blokach:

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
title: Nie widzę żadnych bloków Ruch
---

Jeśli masz wybraną Scenę, to nie zobaczysz żadnych bloków `Ruch`{:class="block3motion"}, ponieważ Scena nie może się poruszać.

Kliknij duszka na Panelu duszków, a następnie kliknij zakładkę **Skrypt**, aby zobaczyć bloki `Ruch`{:class="block3motion"}.

--- /collapse ---

