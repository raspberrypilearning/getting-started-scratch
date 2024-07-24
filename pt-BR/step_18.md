## Debug (Revisando seu código)

**Depurar** é encontrar e corrigir erros em seu código que são chamados de **bugs**.

* É mais fácil identificar problemas se você fizer uma alteração de cada vez e, em seguida, executar seu programa

* Pode levar alguns experimentos para seu projeto funcionar da maneira que você planejou

Aqui estão algumas dicas que podem ajudá-lo a depurar um projeto quando ele não está fazendo o que você deseja:

--- collapse ---
---
title: Executar trechos menores de código
---

Você não precisa executar um programa inteiro para verificar se os últimos blocos novos que você adicionou funcionam.

* Clique em um bloco na área de código para executá-lo - é uma maneira rápida de verificar se um bloco está funcionando conforme o esperado

* Para testar um conjunto de blocos por conta própria, arraste-os para longe do **conteúdo** de seu script, clique neles para testá-los e arraste-os de volta para o script principal

--- /collapse ---

--- collapse ---
---
title: Adicionar atrasos temporários
---

Diminua a **execução** do seu código quando ele for executado. Para fazer isso, adicione um `espere`{:class="block3control"} ou o bloco `espere até que a tecla seja pressionada`{:class="block3control"} e em seguida, remova o bloco quando terminar de depurar seu código.

--- /collapse ---

--- collapse ---
---
title: Mostrar variáveis no Palco
---

Se o seu projeto usa `variáveis`{:class="block3variables"} para armazenar dados, pode ser útil mostrar essas `variáveis`{:class="block3variables"} no Palco.

Clique na caixa de seleção ao lado de uma `variável`{:class="block3variables"} na categoria `Variáveis`{:class="block3variables"} para exibi-la ou ocultá-la no Palco.

A variável sempre tem o valor que você espera?

--- /collapse ---

--- collapse ---
---
title: Adicionar comentários
---

Adicione comentários a blocos, conjuntos de blocos e/ou scripts. Use a linguagem do dia-a-dia para explicar o que o código faz. Às vezes, isso fará com que você perceba que seu código não faz realmente o que você deseja!

Os comentários são úteis quando você deseja entender seu código posteriormente, e ajudam outras pessoas a entender seus projetos.

--- /collapse ---


Existem problemas comuns que muitos iniciantes (e especialistas!) enfrentam no Scratch.

--- collapse ---
---
title: Dicas de depuração para problemas específicos
---

+ **Meu ator está de cabeça para baixo** - Adicione um bloco `defina o estilo de rotação para esquerda-direita`{:class="block3motion"} ou `defina o estilo de rotação para não rotacionar`{:class="block3motion"}.

+ **Meu ator 'pula' quando muda de roupa ou salta** - Certifique-se de que a fantasia esteja centralizada no editor de pintura (alinhe a cruz azul na fantasia com a cruz no centro do editor de pintura).

+ **Meu ator para quando chega à borda do Palco** - Adicione um bloco `se tocar na borda, volte`{:class="block3motion"}.

+ **Meu som não reproduz** - Você adicionou um bloco `toque o som`{:class="block3sound"} quando o ator é clicado? Se você copiou o código de outro ator, você precisará adicionar o som a este ator na categoria **Sons**. Verifique o volume do seu computador ou tablet e certifique-se de que não baixou o volume com o código - tente `mude o volume para`{:class="block3sound"} `100`.

+ **Outros atores continuam na frente do meu ator** - Use um bloco `vá para a camada da frente`{:class="block3looks"}.

+ **Meu ator só se move/muda uma vez** - Coloque seu código dentro de um bloco `sempre`{:class="block3control"} para que ele continue em execução.

+ **Meu ator não muda quando eu movo um controle deslizante variável** - Coloque seu código dentro de um bloco `sempre`{:class="block3control"} para que ele continue atualizando.

--- /collapse ---

**Dica:** Se você não conseguir encontrar o problema depois de tentar essas técnicas, faça uma pausa ou trabalhe em uma parte diferente do seu projeto. Quando você voltar, poderá encontrar o bug imediatamente!

