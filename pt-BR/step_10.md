## Controles

Blocos do tipo `controle`{:class="block3control"} controlam a sequência em que os blocos serão executados, incluindo decisões (seleção) e loops (repetição).


O bloco `espere`{:class="block3control"} coloca um atraso em segundos antes de executar o próximo bloco.

```blocks3
wait (1) seconds// delay for 1 second

wait (0.1) seconds// delay for one tenth of a second
```

Os loops controlam quantas vezes o código que está dentro deles é executado.

```blocks3
repeat (4) // run the blocks inside four time

end
```

```blocks3
forever // run the blocks inside until stopped

end
```

[[[scratch3-forever-condition]]]

**Dica:** Você pode parar a execução de um loop `sempre`{:class="block3events"} clicando no botão Pare acima do Palco, ou usando blocos `pare`{:class="block3control"}.

Existem três opções para o bloco `pare`{:class="block3events"}:

```blocks3
stop [all v] // stop all scripts in all sprites

stop [this script v]

stop [other scripts in sprite v]
```

Os bloco `se...então`{:class="block3control"} e `se...então...senão`{:class="block3control"} são usados para, satisfeita certas condições, saber qual bloco executar em seguida. Isso às vezes é chamado de **seleção**. O bloco `se...então`{:class="block3control"} verifica uma **condição** em forma de hexágono e executa os blocos, se a condição for **verdadeira**. O bloco `se...então...senão`{:class="block3control"} tem uma parte adicional para executar os blocos dentro dele, se a condição for **falsa**.

```blocks3
if <> then

end

if <> then

else

end
```

[[[scratch3-if-then-else]]]

Você pode encontrar blocos em forma hexagonal para usar como condicionadores nas categorias `Operadores`{:class="block3operators"} e `Sensores`{:class="block3sensing"}.

Os blocos `espere até que`{:class="block3control"} e `repita até que`{:class="block3control"} também usam condições:

```blocks3
wait until <> // delay until the condition is true


repeat until <> // repeat the blocks inside until the condtion is true

end
```

Um **clone** é a cópia de um ator, ele contém os trajes, scripts e sons usados pelo ator no momento da clonagem. Existem vários blocos que podem ser usados para clonar atores.

Com o bloco `crie clone de [este ator]`{:class="block3control"}, um ator pode clonar a si mesmo ou um outro ator no projeto.

```blocks3
create clone of [myself v] // clones the sprite that runs this block


create clone of [Butterfly 1 v] // clones another sprite in the project
```

O bloco `quando eu começar como um clone`{:class="block3control"} é usado para executar um novo script uma vez que o clone tenha sido criado. O clone existirá no projeto até que o bloco `apague este clone`{:class="block3control"} seja usado.

Usar o bloco `quando eu começar como um clone`{:class="block3control"} e, em seguida, incluir o bloco `crie clone de [este ator]`{:class="block3control"} no script abaixo significa que também é possível que clones criem outros clones.

```blocks3
when I start as a clone // the script that runs when the clone is created


delete this clone // stops the clone's scripts and deletes it
```

Há um número máximo de clones que um ator pode; até o momento em que este texto está sendo escrito, esse número é `300`.

--- collapse ---
---
title: Clones de clones
---

**Clones**: [Ver interior](https://scratch.mit.edu/projects/567544298/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567544298/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /collapse ---

