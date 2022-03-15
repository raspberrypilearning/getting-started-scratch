## Beweging

Met `Beweging`{:class="block3motion"} blokken kun je je sprite door het Speelveld verplaatsen.

### Verplaatsing

Het `stappen`{:class="block3motion"} blok is de eenvoudigste manier om te beginnen met het verplaatsen van een sprite:

```blocks3
move [10] steps
```

Je kunt met `ga naar`{:class="block3motion"} of `schuif naar`{:class="block3motion"} naar de muisaanwijzer, naar een willekeurige positie op het Speelveld (of je vinger op een tablet) of naar een andere sprite gaan:

```blocks3
go to (random position v)

glide [1] secs to (random position v)
```

Je kunt met `ga naar`{:class="block3motion"} of `schuif naar`{:class="block3motion"} naar `x`{:class="block3motion"} en `y`{:class="block3motion"} coördinaten op het Speelveld gaan.

```blocks3
go to x: [0] y: [0] 

glide [1] secs to x: [0] y: [0]
```

[[[scratch3-glide-to-object]]]

**Tip:** Als je een sprite naar het Speelveld sleept, worden de bewegingsblokken die gebruik maken van `x`{:class="block3motion"} en `y`{:class="block3motion"}-coördinaten bijgewerkt in de `Beweging`{:class="block3motion"} blokken in het menu. De huidige `x`{:class="block3motion"} en `y`{:class="block3motion"} coördinaten worden weergegeven in het Sprite-venster.

### Draaien
Je kunt ook de `richting`{:class="block3motion"} veranderen waar een sprite naar wijst. Dit verandert de richting waarin de sprite zal bewegen als je een `richt naar`{:class="block3motion"} blok gebruikt. Het kan ook de rotatie van het uiterlijk van de sprite veranderen, afhankelijk van de instelling `maak draaistijl`{:class="block3motion"}.

Wanneer je een sprite toevoegt, zal deze naar rechts wijzen (90 graden). Je kunt dit wijzigen in het Sprite-venster of door codeblokken te gebruiken.

```blocks3
turn right [15] degrees

turn left [15] degrees

point in direction [90] // Klik op 90 en sleep de pijl om te wijzigen

point towards (mouse-pointer v)

(direction)

set rotation style [left-right v] // of helemaal rond of niet draaien
```

[[[scratch3-sprite-direction]]]

[[[scratch3-left-right-direction]]]

--- collapse ---
---
title: Ronddraaien
---

--- no-print ---

**Draaiende vleermuis**: [Bekijk van binnen](https://scratch.mit.edu/projects/435704980/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435704980/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Deze code laat een sprite draaien wanneer op de groene vlag wordt geklikt:

```blocks3
when flag clicked
forever
turn right (1) degrees :: motion
```

Verander het aantal graden in `1` in een `draai`{:class="block3motion"} blok binnen een `herhaal`{:class="block3control"} lus, en je sprite blijft draaien.

**Tip:** Als je geen `neem .. stappen`{:class="block3motion"} blok toevoegt, zal je sprite draaien in de positie waarin hij zich bevindt.

--- /collapse ---

--- collapse ---
---
title: Beweeg in een cirkel
---

--- no-print ---

**Beweging van de maan**: [Bekijk van binnen](https://scratch.mit.edu/projects/435701055/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435701055/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Deze code laat een sprite in een cirkel vliegen wanneer op de groene vlag wordt geklikt:

```blocks3
when green flag clicked
forever
move (1) steps
turn right (1) degrees :: motion
```

Verander de waarden in een `neem stappen`{:class="block3motion"} blok en `draai`{:class="block3motion"} blok binnen een `herhaal`{:class="block3control"} blok `1` en je sprite lijkt in een grote cirkel te bewegen.

**Tip:** Als je wilt dat je sprite altijd in het midden van het werkgebied begint, kun je een `ga naar x:`{:class="block3motion"} `0` `y:`{:class="block3motion"} `0` blok toevoegen voor het `herhaal`{:class="block3control"} blok.

--- /collapse --- 

### Stuiteren

Het `keer om aan de rand`{:class="block3motion"}-blok is erg handig als je een sprite wilt laten rondspringen en in het werkgebied wilt houden:

```blocks3
if on edge, bounce
```

Bekijk enkele manieren waarop je je sprite kunt laten rondspringen:

--- collapse ---
---
title: Stuiteren over het Speelveld
---

--- no-print ---

**Meisje dat over het Speelveld beweegt**: [Bekijk van binnen](https://scratch.mit.edu/projects/433535326/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433535326/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Deze code laat een sprite stuiteren op de linker- en rechterrand van het Speelveld. Omdat de sprite horizontaal draait, lijkt hij te kantelen wanneer hij van richting verandert als op de groene vlag wordt geklikt:

```blocks3
when green flag clicked
point in direction (90)
set rotation style [left-right v]
forever
move (5) steps
if on edge, bounce
```

In dit voorbeeld met het `richt naar`{:class="block3motion"}-blok richt de sprite automatisch naar rechts (`90` graden) wanneer op de groene vlag wordt geklikt. Als je het aantal graden verandert in `-90`, zal je sprite naar links wijzen.

Voeg een `maak draaistijl`{:class="block3motion"}-blok toe en selecteer `links-rechts`{:class="block3motion"} in het vervolgkeuzemenu, zodat je sprite niet ondersteboven kantelt wanneer hij stuitert aan de rand van het podium.

**Tip:** Je kunt je sprite in het Speelveld slepen om deze naar de gewenste y-positie (omhoog/omlaag) te verplaatsen.

--- /collapse ---

--- collapse ---
---
title: Op en neer stuiteren over het Speelveld
---

--- no-print ---

**Meisje springt**: [Bekijk van binnen](https://scratch.mit.edu/projects/433595822/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433595822/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Deze code laat een sprite op en neer stuiteren in het Speelveld wanneer op de groene vlag wordt geklikt:

```blocks3
when green flag clicked
point in direction (0)
set rotation style [don't rotate v]
forever
move (5) steps
if on edge, bounce
```

Verander het aantal graden in het `richting naar`{:class="block3motion"} blok naar `0` om een sprite naar boven te laten wijzen.

Voeg een `maak draaistijl`{:class="block3motion"}-blok toe en selecteer `niet draaien`{:class="block3motion"} in het vervolgkeuzemenu om het draaien van je sprite te stoppen, zelfs als deze stuitert.

**Tip:** Je kunt je sprite door het Speelveld slepen om deze naar de gewenste x-positie (links-rechts) te verplaatsen.

--- /collapse ---

--- collapse ---
---
title: Stuiteren onder een hoek
---

--- no-print ---

**Stuiterende voetbal**: [Bekijk van binnen](https://scratch.mit.edu/projects/433536479/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433536479/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Deze code laat een sprite willekeurig draaien wanneer op de groene vlag wordt geklikt:

```blocks3
when green flag clicked
point in direction (45)
set rotation style [all around v]
forever
move (5) steps
if on edge, bounce
```

Als je sprite onder een hoek van `45` graden beweegt, zul je merken dat hij onder een hoek op de rand van het Speelveld lijkt te stuiteren. Verander het aantal graden in het `richt naar`{:class="block3motion"} blok in `45` om je sprite overal rond te laten stuiteren.

Voeg een `maak draaistijl`{:class="block3motion"}-blok toe en selecteer `helemaal rond`{:class="block3motion"} in het vervolgkeuzemenu, zodat je sprite zal draaien wanneer hij stuitert op de rand van het podium.

--- /collapse ---

### Coördinaten gebruiken

Je kunt ook met `verander`{:class="block3motion"} en `maak`{:class="block3motion"} blokken de `x`{:class="block3motion"} en `y`{:class="block3motion"} coördinaten verkrijgen en deze waarden gebruiken in andere blokken:

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
title: Ik zie geen bewegingsblokken
---

Als je het Speelveld hebt geselecteerd zie je geen `Beweging`{:class="block3motion"} blokken, omdat het Speelveld niet kan bewegen.

Klik op een sprite in het Sprite-paneel en klik vervolgens op het **Code** tabblad om de `Beweging`{:class="block3motion"} blokken te zien.

--- /collapse ---

