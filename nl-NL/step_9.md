## Gebeurtenissen

Blokken in het `Gebeurtenissen`{:class="block3events"} menu bepalen wanneer scripts worden gestart.

**Hoed-blokken** voeren de blokken eronder uit wanneer er een bepaalde gebeurtenis plaatsvindt. Ze zijn aan de bovenkant afgerond, zoals een hoed, zodat er geen blokken boven kunnen komen.

Je kunt gebruiken:

```blocks3

when flag clicked // blokken uitvoeren wanneer op de groene vlag boven het speelveld wordt geklikt

when this sprite clicked // voer de blokken uit wanneer op de sprite voor dit script wordt geklikt

when stage clicked // voer de blokken uit wanneer op het speelveld wordt geklikt

```

**Tip:** Het `wanneer op het Speelveld wordt geklikt`{:class="block3events"} is alleen beschikbaar wanneer je in het codegebied voor het Speelveld werkt.

Als je op een computer met een toetsenbord werkt, kun je de `wanneer toets is ingedrukt`{:class="block3events"} gebruiken:

```blocks3
when [space v] key pressed // wijzigen naar cijfer-, letter- of pijltoetsen
```

Je kunt ook een `wanneer achtergrond verandert naar`{:class="block3events"} blok gebruiken om een script te starten wanneer de achtergrond verandert.

[[[scratch3-changing-backdrops-pages-levels]]]

[[[scratch3-show-hide-sprites-backdrops]]]


Het `wanneer >`{:class="block3events"} blok heeft twee versies:

```blocks3
when [loudness v] > (10) // blokken uitvoeren wanneer de microfoon geluid detecteert

when [timer v] > (10) // blokken uitvoeren wanneer de timer 10 seconden bereikt
```

[[[scratch3-time-delay]]]


De laatste twee blokken in het `Gebeurtenissen`{:class="block3events"} menu zijn `zend signaal`{:class="block3events"} blokken. Je kunt `wanneer ik signaal ontvang`{:class="block3events"} gebruiken om een script te starten wanneer een sprite een overeenkomend `zend signaal`{:class="block3events"}-blok uitvoert.

[[[generic-scratch3-broadcast-message]]]

