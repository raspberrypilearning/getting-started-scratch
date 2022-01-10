## Operadores

The `Operators`{:class="block3operators"} blocks are used to compare variables and values, do calculations with numbers, and work with strings (text).

Los bloques hexagonales 'booleanos' se utilizan como condiciones y devuelven verdadero o falso. Estos bloques se pueden utilizar en bloques `Control`{:class="block3control"} con una entrada hexagonal.

Operadores de comparación:

```blocks3
<[] > [50]>

<[] < [50]>

<[] = [50]>
```

**Consejo:** Cuando uses `=`{:class="block3operators"} con texto puedes mezclar letras mayúsculas y minúsculas, por lo que `<`{:class="block3operators"} `SI` `=`{:class="block3operators"} `si` `>`{:class="block3operators"} devuelve **verdadero**.


Hay operaciones matemáticas:

```blocks3
([] + [])

([] - [])

([] * [])

([] / [])
```

Puedes elegir números aleatorios entre el número más pequeño y el más grande (incluidos esos números).

```blocks3
(pick random [1] to [10]) // A number from 1 to 10
```

The `and`{:class="block3operators"}, `or`{:class="block3operators"}, and `not`{:class="block3operators"} operators can be used to combine conditions.

```blocks3
<<> and <>>

<<> or <>>

<not <> >
```

Hay bloques para trabajar con cadenas de texto:

```blocks3
(join [apple ] [banana])

(letter [1] of [apple])

(length of [apple])

<[apple] contains [a]>
```

[[[scratch3-join-text]]]

También hay más operadores matemáticos que son útiles para algunos proyectos.
