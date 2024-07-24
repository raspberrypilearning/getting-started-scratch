## Eventos

Blocos da categoria `Eventos`{:class="block3events"} do menu controlam quando os scripts são iniciados.

**Blocos chapéu** executam o código abaixo deles quando um evento em particular acontece. Eles são arredondados na parte superior, como um chapéu, então nenhum bloco pode passar por cima deles.

Você pode usar:

```blocks3

when flag clicked // executa os blocos quando a bandeira verde acima do Palco é clicada

when this sprite clicked // executa os blocos quando o personagem dessa animação é clicado

when stage clicked // executa os blocos quando o palco for clicado

```

**Dica:** O bloco `quando palco for clicado`{:class="block3events"} está disponível somente quando você estiver trabalhando na área do Código para o Palco.

Se você estiver em um computador com teclado, você pode usar o bloco `quando a tecla for pressionada`{:class="block3events"}:

```blocks3
when [espaço v] key pressed // muda para número, letra ou setas de direção
```

Você pode também usar o bloco `quando o cenário mudar para`{:class="block3events"} para iniciar um script quando o cenário mudar.

[[[scratch3-changing-backdrops-pages-levels]]]

[[[scratch3-show-hide-sprites-backdrops]]]


O bloco `quando >` tem duas versões:

```blocks3
when [ruído v] > (10) // executa blocos quando o microfone detectar som

when [cronômetro v] > (10) // executa blocos quando o cronômetro chegar a 10 segundos
```

[[[scratch3-time-delay]]]


Os últimos dois blocos no menu `Eventos`{:class="block3events"} são blocos `broadcast`{:class="block3events"}. Você pode usar um bloco `quando eu receber (message v)`{:class="block3events"} para iniciar um script quando qualquer ator executar o bloco `transmita (message v)`{:class="block3events"} correspondente.

[[[generic-scratch3-broadcast-message]]]

