## Besturen

`Besturen`{:class="block3control"} blokken bepalen de volgorde waarin blokken worden uitgevoerd, inclusief beslissingen (keuzes) en lussen (herhaling).


Het `wacht`{:class="block3control"} blok vertraagt een aantal seconden voordat het volgende blok wordt uitgevoerd.

```blocks3
wait (1) seconds// delay for 1 second

wait (0.1) seconds// delay for one tenth of a second
```

Lussen bepalen hoe vaak de code erin wordt uitgevoerd.

```blocks3
repeat (4) // run the blocks inside four time

end
```

```blocks3
forever // run the blocks inside until stopped

end
```

[[[scratch3-forever-condition]]]

**Tip:** Je kunt een `herhaal`{:class="block3events"}-blok stoppen door op de rode Stop knop boven het Speelveld te klikken, of door de `stop`{:class="block3control"}-blokken te gebruiken.

Er zijn drie opties voor het `stop`{:class="block3events"} blok:

```blocks3
stop [all v] // stop all scripts in all sprites

stop [this script v]

stop [other scripts in sprite v]
```

De `als...dan`{:class="block3control"} en `als...dan...anders`{:class="block3control"} blokken worden gebruikt om aan te geven welke codeblokken als volgende moeten worden uitgevoerd. Dit wordt soms **selectie** genoemd. Het `als...dan`{:class="block3control"} blok controleert een zeshoekige **voorwaarde** en voert de ingesloten codeblokken uit, als de voorwaarde **waar** is. Het `als...dan..anders`{:class="block3control"} blok heeft een extra sectie om de ingesloten codeblokken uit te voeren, als de voorwaarde **niet waar** is.

```blocks3
if <> then

end

if <> then

else

end
```

[[[scratch3-if-then-else]]]

Je kunt zeshoekige blokken vinden die je als voorwaarden kunt gebruiken in de `Functies`{:class="block3operators"} en `Waarneming`{:class="block3sensing"} blokken.

De `wacht tot`{:class="block3control"} en `herhaal tot`{:class="block3control"} blokken gebruiken ook voorwaarden:

```blocks3
wait until <> // delay until the condition is true


repeat until <> // repeat the blocks inside until the condtion is true

end
```

Een **kloon** is een kopie van een sprite, het heeft het uiterlijk, scripts en geluiden van de sprite waaruit het is gekloond op het moment van klonen. Er zijn een aantal blokken die gebruikt kunnen worden om sprites te klonen.

Met de `maak een kloon van [mijzelf v]`{:class="block3control"} blok, kan een sprite een kloon van zichzelf of van een andere sprite in het project maken.

```blocks3
create clone of [myself v] // clones the sprite that runs this block


create clone of [Butterfly 1 v] // clones another sprite in the project
```

Het `wanneer ik als kloon start`{:class="block3control"} hoed-blok wordt gebruikt om een nieuw script te activeren zodra de kloon is gemaakt. De kloon zal in het project blijven bestaan totdat het `verwijder deze kloon`{:class="block3control"} sluit-blok wordt gebruikt.

Het `wanneer ik als kloon start`{:class="block3control"} hoed-blok en vervolgens het blok `maak een kloon van [mijzelf v]`{:class="block3control"} opnemen in het onderstaande script betekent dat ook klonen andere klonen kunnen maken.

```blocks3
when I start as a clone // the script that runs when the clone is created


delete this clone // stops the clone's scripts and deletes it
```

Er is een maximum aantal klonen dat een sprite op elk moment kan hebben, op dit moment is dat `300`.

--- collapse ---
---
title: Klonen van klonen
---

**Klonen**: [Bekijk van binnen](https://scratch.mit.edu/projects/567544298/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567544298/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /collapse ---

