## Operators

The `Operators`{:class="block3operators"} blocks are used to compare variables and values, do calculations with numbers and work with strings (text).

The hexagonal 'Boolean' blocks are used as conditions and return true or false and can be used in `Control`{:class="block3control"} blocks with a hexagonal input.

Comparison operators:

```blocks3
<[] > [50]>

<[] < [50]>

<[] = [50]>
```

**Tip:** When you use `=`{:class="block3operators"} with text you can mix upper and lowercase letters, so `<`{:class="block3operators"}YES` `=`{:class="block3operators"} `yes``>`{:class="block3operators"} returns **true**.


There are maths operations:

```blocks3
([] + [])

([] - [])

([] * [])

([] / [])
```

You can choose random numbers between the smallest and largest number (including those numbers).

```blocks3
(pick random [1] to [10]) // A number from 1 to 10
```

The `and`{:class="block3operators"}, `or`{:class="block3operators"} and `not`{:class="block3operators"} operators can be used to combine comditions.

```blocks3
<<> and <>>

<<> or <>>

<not <> >
```

There are blocks for working with text strings:

```blocks3
(join [apple ] [banana])

(letter [1] of [apple])

(length of [apple])

<[apple] contains [a]>
```

[[[scratch3-join-text]]]

There are also more maths operators that are useful for some projects.