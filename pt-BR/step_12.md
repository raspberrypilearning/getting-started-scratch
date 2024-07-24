## Operadores

Os blocos da categoria `Operadores`{:class="block3operators"} são usados para comparar variáveis e valores, fazer cálculos com números e trabalhar com strings (texto).

Os blocos hexagonais 'Booleanos' são usados como condições e retornam verdadeiro ou falso. Esses blocos podem ser usado em blocos da categoria `Controle`{:class="block3control"} com uma entrada hexagonal.

Operadores de comparação:

```blocks3
<[] > [50]>

<[] < [50]>

<[] = [50]>
```

**Dica:** Quando você usa`=`{:class="block3operators"} com texto, você pode misturar letras maiúsculas e minúsculas, assim`<`{:class="block3operators"} `SIM` `=`{:class="block3operators"} `sim` `>`{:class="block3operators"} retorna **verdadeiro**.


Existem operações matemáticas:

```blocks3
([] + [])

([] - [])

([] * [])

([] / [])
```

Você pode escolher números aleatórios entre o menor e o maior número (incluindo esses números).

```blocks3
(pick random [1] to [10]) // Um número entre 1 e 10
```

Os operadores `e`{:class="block3operators"}, `ou`{:class="block3operators"}, e `não`{:class="block3operators"} podem ser usados para combinar condições.

```blocks3
<<> and <>>

<<> or <>>

<not <> >
```

Existem blocos para trabalhar com strings de texto:

```blocks3
(join [maçã ] [banana])

(letter [1] of [maçã])

(length of [maçã])

<[maçã] contains [a]>
```

[[[scratch3-join-text]]]

Existem também mais operadores matemáticos que são úteis para alguns projetos.
