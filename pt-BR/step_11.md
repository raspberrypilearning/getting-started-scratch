## Sensores

Os blocos no menu `Sensores`{:class="block3sensing"} são usados para obter textos do usuário, detectar condições e relatar valores em seu projeto.

Existem vários blocos hexagonais na categoria `Sensores`{:class="block3sensing"} que você pode usar em blocos da categoria `Controle`{:class="block3control"} para tomar decisões e controlar quando os blocos são executados.

O bloco `tocando em`{:class="block3sensing"} tem opções para detectar se o ator que possui seu próprio script está tocando o ponteiro do mouse (onde seu dedo tocou por último na tela do tablet), na borda do Palco, ou um outro ator:

```blocks3
<touching (mouse-pointer v) ?>

<touching (edge v) ?>

<touching (Sprite2 v) ?>
```

Existem blocos para detectar se o ator que possui seu próprio script está tocando em outra cor (no Palco ou em outro ator), ou se uma cor neste ator está tocando em outra cor.

```blocks3
<touching color (#c5a97b) ?>

<color (#c219ed) is touching (#62d1e0) ?>
```

A bloco `tecla pressionada`bloco{:class="block3sensing"} tem opções para números, letras e setas de direção. Você precisa de um teclado para pressionar as teclas. Ele detecta se uma tecla está sendo pressionada:

```blocks3
<key (space v) pressed?>
```

O bloco `mouse pressionado`{:class="block3sensing"} detecta se o mouse está sendo pressionado no momento ou se a tela está sendo tocada em uma tela sensível ao toque:

```blocks3
<mouse down?>
```

Os blocos `pergunte e espere`{:class="block3sensing"} e `resposta`{:class="block3sensing"} são usados para obter texto do usuário:

```blocks3
ask [What's your name] and wait

(answer) // the text the the user typed 
```

O bloco `perguntar`{:class="block3sensing"} funciona com um teclado ou com um teclado virtual na tela de um tablet.

O bloco `resposta`{:class="block3sensing"} é um bloco que informa um valor e pode ser usado como uma variável.

[[[scratch3-ask-answer-chat]]]

O menu `Sensores`{:class="block3sensing"} tem vários blocos que podem ser usados para obter ou informar valores:

```blocks3
(distance to (mouse-pointer v))

(distance to (Sprite2 v))
```

Você pode detectar a posição atual do ponteiro do mouse (ou a posição atual ou mais recente do seu dedo em um tablet):

```blocks3
(mouse x)

(mouse y)
```

Você pode detectar a `ruído`{:class="block3sensing"} do som do microfone. Uma janela pop-up solicitará permissão ao usuário para usar o microfone:

```blocks3
(loudness)
```

O bloco `cronômetro`{:class="block3sensing"} começa a contar quando o projeta começa a carregar, e pode ser redefinido para `0` com `zere o cronômetro`{:class="block3sensing"}:

```blocks3
(timer)

reset timer
```

Você também pode acessar blocos que informam para o Palco e outros atores:

```blocks3
([backdrop # v] of (_stage_ v))

([x position v] of (Sprite2 v))

([costume # v] of (Sprite2 v))
```

Existem blocos que informam informações relacionadas à data e hora no mundo real, em seu fuso horário local:

```blocks3
(current [year v]) // hour, minute, ...

(days since 2000)
```

