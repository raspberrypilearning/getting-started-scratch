## Fouten oplossen (Debuggen)

**Debuggen** is het vinden en herstellen van fouten in je code. Fouten worden **bugs** genoemd.

* Het is gemakkelijker om problemen te vinden als je één wijziging tegelijk aanbrengt en vervolgens je programma uitvoert

* Het kan een paar aanpassingen duren voordat je project werkt zoals je het gepland had

Hier zijn enkele tips die je kunnen helpen bij het debuggen van een project wanneer het niet doet wat je wilt:

--- collapse ---
---
title: Voer kleinere stukjes code uit
---

Je hoeft niet een heel programma uit te voeren om te controleren of de laatste paar nieuwe blokken die je hebt toegevoegd werken.

* Klik op een blok in het werkgebied om het uit te voeren - het is een snelle manier om te controleren of een blok werkt zoals je verwacht

* Om zelf een set blokken te testen, sleep je ze weg van hun **hoofd** script, klik erop om ze te testen en sleep ze vervolgens terug naar het hoofdscript

--- /collapse ---

--- collapse ---
---
title: Tijdelijke vertragingen toevoegen
---

Vertraag de **uitvoering** van je code wanneer deze wordt uitgevoerd. Om dit te doen, voeg je een `wacht`{:class="block3control"} of `wacht tot toets is ingedrukt`{:class="block3control"} blok toe en verwijder het blok weer wanneer je klaar bent met het debuggen van je code.

--- /collapse ---

--- collapse ---
---
title: Variabelen in het Speelveld tonen
---

Als je project `variabelen`{:class="block3variables"} gebruikt om gegevens op te slaan, kan het handig zijn om die `variabelen`{:class="block3variables"} in het Speelveld weer te geven.

Klik op het selectievakje naast een `variabele`{:class="block3variables"} in het `Variabelen`{:class="block3variables"} blokkenmenu om deze in het Speelveld te tonen of te verbergen.

Heeft de variabele altijd de waarde die je verwacht?

--- /collapse ---

--- collapse ---
---
title: Opmerkingen toevoegen
---

Voeg opmerkingen toe aan blokken, sets met blokken en/of scripts. Gebruik alledaagse taal om uit te leggen wat de code doet. Soms kom je er daardoor achter dat je code niet echt doet wat je wilt!

Opmerkingen zijn handig als je jouw code later wilt begrijpen en ze helpen ook andere mensen om jouw projecten te begrijpen.

--- /collapse ---


Er zijn veelvoorkomende problemen die veel beginners (en experts!) tegenkomen in Scratch.

--- collapse ---
---
title: Foutopsporings-tips voor specifieke problemen
---

+ **Mijn sprite gaat ondersteboven** — Voeg een `maak draaistijl links-rechts`{:class="block3motion"} of `maak draaistijl niet draaien`{:class="block3motion"} blok toe.

+ **Mijn sprite 'springt' wanneer het van uiterlijk verandert of stuitert** — Zorg ervoor dat het uiterlijk gecentreerd is in de Teken-editor (zet het blauwe kruis in het uiterlijk in het midden van de Teken-editor op het dradenkruis).

+ **Mijn sprite stopt wanneer hij de rand van het Speelveld raakt** — Voeg een `keer om aan de rand`{:class="block3motion"} blok toe.

+ **Mijn geluid speelt niet af** — Heb je een blok `start geluid`{:class="block3sound"} toegevoegd wanneer op de sprite wordt geklikt? Als je code van een andere sprite hebt gekopieerd, moet je het geluid aan deze sprite toevoegen in het tabblad **Geluiden**. Controleer het volume op je computer of tablet en zorg ervoor dat je het volume niet met code hebt verlaagd — probeer `zet volume op`{:class="block3sound"} `100`.

+ **Andere sprites blijven voor mijn sprite gaan** — Gebruik een `ga naar laag voorgrond`{:class="block3looks"}-blok.

+ **Mijn sprite beweegt/verandert maar één keer** — Zet je code in een `herhaal`{:class="block3control"}- blok zodat het blijft herhalen.

+ **Mijn sprite verandert niet wanneer ik een variabele schuifregelaar verplaats** — Plaats je code in een `herhaal`{:class="block3control"}-blok zodat het blijft updaten.

--- /collapse ---

**Tip:** Als je het probleem niet kunt vinden nadat je deze technieken hebt uitgeprobeerd, neem dan een pauze of werk aan een ander deel van je project. Als je terugkomt, vind je de bug misschien meteen!

