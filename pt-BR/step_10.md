## Controles

Blocos do tipo `controle`{:class="block3control"} controlam a sequência em que os blocos serão executados, incluindo decisões (seleção) e loops (repetição).


O bloco `espere`{:class="block3control"} coloca um atraso em segundos antes de executar o próximo bloco.

```blocks3
wait (1) seconds// atraso de 1 segundo

wait (0.1) seconds// atraso de um décimo de segundo
```

Os loops controlam quantas vezes o código que está dentro deles é executado.

```blocks3
repeat (4) // executa quatro vezes os blocos posicionados dentro

end
```

```blocks3
forever // executa os blocos posicionados dentro até ser parado

end
```

[[[scratch3-forever-condition]]]

**Dica:** Você pode parar a execução de um loop `sempre`{:class="block3events"} clicando no botão Pare acima do Palco, ou usando blocos `pare`{:class="block3control"}.

Existem três opções para o bloco `pare`{:class="block3events"}:

```blocks3
stop [todos v] // para todos os scripts em todos os atores

stop [este script v]

stop [outros scripts no ator v]
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
wait until <> // atrasa até que a condição seja verdadeira


repeat until <> // repete os blocos posicionados dentro até que a condição seja verdadeira

end
```

Um **clone** é a cópia de um ator, ele contém os trajes, scripts e sons usados pelo ator no momento da clonagem. Existem vários blocos que podem ser usados para clonar atores.

Com o bloco `crie clone de [este ator]`{:class="block3control"}, um ator pode clonar a si mesmo ou um outro ator no projeto.

```blocks3
create clone of [este ator v] // cria uma cópia do ator que executa este bloco

create clone of [Butterfly 1 v] // cria uma cópia de um outro ator no projeto
```

O bloco `quando eu começar como um clone`{:class="block3control"} é usado para executar um novo script uma vez que o clone tenha sido criado. O clone existirá no projeto até que o bloco `apague este clone`{:class="block3control"} seja usado.

Usar o bloco `quando eu começar como um clone`{:class="block3control"} e, em seguida, incluir o bloco `crie clone de [este ator]`{:class="block3control"} no script abaixo significa que também é possível que clones criem outros clones.

```blocks3
when I start as a clone // o script que é executado quando a cópia é criada


delete this clone // para e deleta os scripts das cópias
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

