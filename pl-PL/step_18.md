## Debugowanie

**Debugowanie** (czytaj: debagowanie) to znajdowanie i naprawianie błędów w kodzie.

* Łatwiej jest zidentyfikować problemy, jeśli dokonasz tylko jednej zmiany, a następnie uruchomisz program

* To może wymagać kilku prób, aby Twój projekt zadziałał w zaplanowany sposób

Oto kilka wskazówek, które mogą pomóc w debugowaniu projektu, gdy nie robi on tego, czego chcesz:

--- collapse ---
---
title: Uruchom mniejsze fragmenty kodu
---

Nie musisz uruchamiać całego programu aby sprawdzić, czy kilka ostatnich bloków, które ostatnio dodałeś, działa poprawnie.

* Kliknij blok w Obszarze kodu, aby go uruchomić — jest to szybki sposób na sprawdzenie, czy blok działa zgodnie z oczekiwaniem

* Aby samodzielnie przetestować zestaw bloków, przeciągnij je poza **zawierający** je skrypt, kliknij je, aby je przetestować, a następnie przeciągnij je z powrotem do głównego skryptu

--- /collapse ---

--- collapse ---
---
title: Dodaj tymczasowe opóźnienia
---

Spowolnij **wykonanie** kodu, gdy jest on uruchamiany. Aby to zrobić, dodaj `czekaj`{:class="block3control"} lub `czekaj, aż klawisz naciśnięty`{:class="block3control"}, a następnie usuń ten blok po zakończeniu debugowania kodu.

--- /collapse ---

--- collapse ---
---
title: Pokaż zmienne na Scenie
---

Jeśli Twój projekt używa `zmiennych`{:class="block3variables"} do przechowywania danych, pomocne może być pokazanie tych `zmiennych`{:class="block3variables"} na Scenie.

Kliknij pole wyboru obok bloku `zmienna`{:class="block3variables"} w menu bloków `Zmienne`{:class="block3variables"}, aby pokazać lub ukryć ją na Scenie.

Czy zmienna zawsze ma taką wartość, jakiej się spodziewasz?

--- /collapse ---

--- collapse ---
---
title: Dodaj komentarze
---

Dodaj komentarze do bloków, zestawów bloków i/lub skryptów. Użyj prostego języka do wyjaśnienia, co robi kod. Czasami dzięki temu zdasz sobie sprawę, że Twój kod nie robi tego, czego od niego oczekujesz!

Komentarze są przydatne, gdy chcesz później zrozumieć swój kod oraz pomagają innym osobom zrozumieć Twoje projekty.

--- /collapse ---


Istnieją typowe problemy, z którymi spotyka się wielu początkujących (i ekspertów!) w Scratchu.

--- collapse ---
---
title: Wskazówki do usuwania konkretnych problemów
---

+ **Mój duszek porusza się do góry nogami** — Dodaj blok `ustaw styl obrotu na lewo-prawo`{:class="block3motion"} lub `ustaw styl obrotu na nie obracaj`{:class="block3motion"}.

+ **Mój duszek „podskakuje”, gdy zmienia kostium lub się odbija** — Upewnij się, że kostium jest wyśrodkowany w edytorze Paint (wyrównaj niebieski krzyż w kostiumie z celownikiem na środku edytora Paint).

+ **Mój duszek zatrzymuje się, gdy dojdzie do krawędzi Sceny** - Dodaj blok `jeżeli na brzegu, odbij się`{:class="block3motion"}.

+ **Mój dźwięk nie jest odtwarzany** — Czy dodałeś blok `graj dźwięk`{:class="block3sound"} po kliknięciu duszka? Jeśli skopiowałeś kod z innego duszka, będziesz musiał dodać dźwięk do tego duszka w zakładce **Dźwięki**. Sprawdź głośność na komputerze lub tablecie i upewnij się, że nie obniżyłeś głośności kodem — spróbuj bloku `ustaw głośność na`{:class="block3sound"} `100`.

+ **Inne duszki zakrywają mojego duszka** — Użyj bloku `przesuń na wierzch`{:class="block3looks"}.

+ **Mój duszek porusza się/zmienia się tylko raz** — Umieść swój kod w bloku `zawsze`{:class="block3control"}, aby poruszał bez przerwy.

+ **Mój duszek nie zmienia się, gdy przesuwam suwak zmiennej** — Umieść swój kod w bloku `zawsze`{:class="block3control"}, aby był na bieżąco aktualizowany.

--- /collapse ---

**Wskazówka:** Jeśli nie możesz znaleźć problemu po wypróbowaniu tych technik, zrób sobie przerwę lub popracuj nad inną częścią projektu. Kiedy wrócisz, być może od razu znajdziesz błąd!

