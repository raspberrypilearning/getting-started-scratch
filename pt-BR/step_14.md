## Meus blocos

`Meus blocos`{:class="block3myblocks"} permite que você crie novos blocos para um ator. Você dá um nome ao bloco e então `define`{:class="block3myblocks"} o que o novo bloco faz usando outros blocos no Scratch. Você pode usar um novo bloco em qualquer script no ator que possui bloco.

Este exemplo define um bloco `conversar`{:class="block3myblocks"} que faz um ator mudar o traje:

**Pinguim gorjeia**: [Ver interior](https://scratch.mit.edu/projects/567554899/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567554899/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

```blocks3
define fala
switch costume to (penguin2-b v)
repeat (2)
play sound (chirp v) until done
end
switch costume to (penguin2-a v)

when this sprite clicked
fala

when [espaço v] key pressed
fala
```

Você pode usar `Meus Blocos`{:class="block3myblocks"} para **organizar** o seu código. É mais simples agrupar todos os blocos que fazem um ator falar e então apenas usar um bloco `falar`{:class="block3myblocks"} quando você quer que seu ator fale.

Se você decidir mudar a forma com que seu ator fala então você tem que alterar o código somente em um lugar.

### Meus blocos com entradas

Você pode também adicionar **entradas** a `Meus blocos`{:class="block3myblocks"} para que eles usem os valores que você entra quando usar o bloco.

**Pinguim fala**: [Ver interior](https://scratch.mit.edu/projects/567538874/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567538874/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

```blocks3
define fala (palavras)
switch costume to (penguin2-b v)
say (palavras) // usa a entrada fornecida
repeat (2)
play sound (chirp v) until done
end
say (palavras)
switch costume to (penguin2-a v)

when this sprite clicked
fala [olá]

when [espaço v] key pressed
fala [oi]
```

[[[generic-scratch3-make-block]]]

--- collapse ---
---
title: Use Meus blocos para organizar o código
---
A forma mais simples de usar `Meus blocos`{:class="block3myblocks"} é para ajudar você a organizar o código. Aqui está um exemplo simples.

```blocks3
define move right
if <not <touching (borda v) ?>> then
switch costume to [direita_1 v]
change x by (2)
switch costume to [direita_2 v]
change x by (2)
switch costume to [direita_3 v]
change x by (2)
end

define move left
if <not <touching (borda v) ?>> then
switch costume to [esquerda_1 v]
change x by (-2)
switch costume to [esquerda_2 v]
change x by (-2)
switch costume to [esquerda_3 v]
change x by (-2)
end

when flag clicked
forever
if <key (seta para direita v) pressed> then
move right
end
if <key (seta para esquerda v) pressed> then
move left
```

--- /collapse ---

`Meus blocos`{:class="block3myblocks"} são similares a 'procedimentos', 'funções' ou 'métodos' em outras linguagens de programação.
