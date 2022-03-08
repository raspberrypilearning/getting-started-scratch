## Movimento

Os blocos de `Movimento`{:class="block3motion"} permitem que você mova o seu ator pelo Palco.

### Movimento

O bloco `mova`{:class="block3motion"} é a maneira mais fácil de começar a mover um ator:

```blocks3
move [10] steps
```

Você pode `mover`{: class = "block3motion"} ou `deslizar`{: class = "block3motion"} o ponteiro do mouse, em uma posição aleatória no Palco (ou seu dedo em um tablet) ou outro ator:

```blocks3
go to (random position v)

glide [1] secs to (random position v)
```

Você também pode `mover`{: class = "block3motion"} ou `deslizar`{: class = "block3motion"} a uma determinada posição de coordenadas `x`{: class = "block3motion"} e `y`{: class = "block3motion"} no Palco.

```blocks3
go to x: [0] y: [0] 

glide [1] secs to x: [0] y: [0]
```

[[[scratch3-glide-to-object]]]

**Dica:** Quando você arrasta um ator sobre o Palco, os blocos de movimentos que usam as coordenadas `x`{:class="block3motion"} e `y`{:class="block3motion"} atualizam na categoria `Movimento x: y:`{:class="block3motion"} do menu de blocos. As coordenadas atuais `x`{:class="block3motion"} e `y`{:class="block3motion"} são mostradas no painel do Ator.

### Rotação
Você também pode alterar a `direção`{: class = "block3motion"} para a qual um ator está apontando. Isso muda a direção em que o ator moverá se você usar o bloco `mova`{: class = "block3motion"}. Também pode-se alterar a rotação da fantasia do ator dependendo da configuração do `estilo de rotação`{: class = "block3motion"}.

Quando você adiciona um ator, ele estará voltado para a direita (90 graus). Você pode alterar isso no painel do Ator ou usando blocos de código.

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
título: Girar
---

--- no-print ---

**Morcego giratório**: [Ver interior](https://scratch.mit.edu/projects/435704980/editor){: target="_ blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435704980/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Este código faz um ator girar quando a bandeira verde é clicada:

```blocks3
when flag clicked
forever
turn right (1) degrees :: motion
```

Em um bloco `gire`{: class = "block3motion"} dentro de um loop `sempre`{: class = "block3control"}, altere o número de graus para `1` e seu ator girará.

**Dica:** Se você não adicionar um bloco `mova`{: class = "block3motion"}, seu ator vai girar na posição em que está.

--- /collapse ---

--- collapse ---
---
título: Mover em um círculo
---

--- no-print ---

**Lua em órbita**: [Ver interior](https://scratch.mit.edu/projects/435701055/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435701055/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Este código faz um ator voar em círculos quando a bandeira verde é clicada:

```blocks3
when green flag clicked
forever
move (1) steps
turn right (1) degrees :: motion
```

Altere os valores nos blocos `mova`{: class = "block3motion"} e `gire`{: class = "block3motion"} dentro de um bloco `sempre`{: class = "block3control"} para `1` e seu ator parecerá se mover em um grande círculo.

**Dica:** Se você quiser que seu ator sempre comece no centro do palco, você pode adicionar um bloco `vá para x:`{:class="block3motion"} `0` e `y:`{:class="block3motion"} `0` antes do bloco `sempre`{:class="block3control"}.

--- /collapse ---

### Virando

O bloco `Se tocar na borda, volte`{: class = "block3motion"} é realmente útil quando você deseja fazer um ator voltar e permanecer no Palco:

```blocks3
if on edge, bounce
```

Veja algumas das maneiras pelas quais você pode fazer seu ator virar:

--- collapse ---
---
título: Virar de um lado do Palco ao outro
---

--- no-print ---

**Garota se movendo pelo Palco**: [Veja interior](https://scratch.mit.edu/projects/433535326/editor){: target = "_ blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433535326/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Este código faz um ator mover pelas bordas esquerda e direita do Palco. Como o ator gira horizontalmente, quando a bandeira verde é clicada ele parece virar quando muda de direção:

```blocks3
when green flag clicked
point in direction (90)
set rotation style [left-right v]
forever
move (5) steps
if on edge, bounce
```

Neste exemplo, o `aponte para a direção`{: class = "block3motion"} automaticamente aponta o ator para a direita (`90` graus) quando a bandeira verde é clicada. Se você alterar o número de graus para `-90`, seu ator apontará para a esquerda.

Adicione um bloco `defina o estilo de rotação para`{: class = "block3motion"} e selecione `esquerda-direita`{: class = "block3motion"} no menu suspenso, de modo que seu ator não vire de cabeça para baixo quando saltar na borda do Palco.

**Dica:** Você pode arrastar seu ator no Palco para movê-lo para a posição y (cima – baixo) desejada.

--- /collapse ---

--- collapse ---
---
título: Pulando pelo palco
---

--- no-print ---

**Menina pulando**: [Veja interior](https://scratch.mit.edu/projects/433595822/editor){: target = "_ blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433595822/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Este código faz um ator pular no palco quando a bandeira verde é clicada:

```blocks3
when green flag clicked
point in direction (0)
set rotation style [don't rotate v]
forever
move (5) steps
if on edge, bounce
```

Altere o número de graus no bloco `aponte para a direção`{: class = "block3motion"} para `0` para fazer um ator apontar para cima.

Adicione um bloco `defina o estilo de rotação para`{: class = "block3motion"} e selecione `não rotacionar`{: class = "block3motion"} no menu suspenso para seu ator não rotacionar, mesmo quando ele pula.

**Dica:** Você pode arrastar seu ator pelo Palco para movê-lo para a posição x (esquerda-direita) desejada.

--- /collapse ---

--- collapse ---
---
título: Pular em ângulo
---

--- no-print ---

**Football bouncing**: [See inside](https://scratch.mit.edu/projects/433536479/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433536479/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

This code makes a sprite appear to rotate randomly when the green flag is clicked:

```blocks3
when green flag clicked
point in direction (45)
set rotation style [all around v]
forever
move (5) steps
if on edge, bounce
```

If your sprite moves at `45` degrees, you will find that it appears to bounce on the edge of the Stage at an angle. Change the number of degrees in the `point in direction`{:class="block3motion"} block to `45` to make your sprite bounce all around.

Add a `set rotation style`{:class="block3motion"} block and select `all around`{:class="block3motion"} in the drop-down menu, so that your sprite will turn when it bounces on the edge of the Stage.

--- /collapse ---

### Using coordinates

You can also `change`{:class="block3motion"} and `set`{:class="block3motion"} the `x`{:class="block3motion"} and `y`{:class="block3motion"} coordinates and get their values to use in other blocks:

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
title: I can't see any Motion blocks
---

If you have the Stage selected then you won't see any `Motion`{:class="block3motion"} blocks, because the Stage can't move.

Click on a sprite in the Sprite pane and then click on the **Code** tab to see the `Motion`{:class="block3motion"} blocks.

--- /collapse ---

