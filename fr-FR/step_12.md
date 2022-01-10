## Opérateurs

Les blocs `Opérateurs`{:class="block3operators"} sont utilisés pour comparer des variables et des valeurs, effectuer des calculs numériques et travailler avec des chaînes de caractères (texte).

Les blocs 'booléens' hexagonaux sont utilisés comme conditions et renvoient vrai ou faux. Ces blocs peuvent être utilisés dans des blocs `Contrôle`{:class="block3control"} possédant une entrée hexagonale.

Opérateurs de comparaison :

```blocks3
<[] > [50]>

<[] < [50]>

<[] = [50]>
```

**Astuce :** Lorsque tu utilises `=`{:class="block3operators"} avec du texte, tu peux mélanger des lettres majuscules et minuscules, donc `<`{:class="block3operators"} `OUI` `=`{:class ="block3operators"} `oui` `>`{:class="block3operators"} renvoie **vrai**.


Il existe des opérations mathématiques :

```blocks3
([] + [])

([] - [])

([] * [])

([] / [])
```

Vous pouvez tirer des nombres aléatoires entre le plus petit et le plus grand nombre (ces nombres y compris).

```blocks3
(pick random [1] to [10]) // A number from 1 to 10
```

Les opérateurs `et`{:class="block3operators"}, `ou`{:class="block3operators"} et `non`{:class="block3operators"} peuvent être utilisés pour combiner des conditions.

```blocks3
<<> and <>>

<<> or <>>

<not <> >
```

Il existe des blocs pour travailler avec des chaînes de caractères :

```blocks3
(join [apple ] [banana])

(letter [1] of [apple])

(length of [apple])

<[apple] contains [a]>
```

[[[scratch3-join-text]]]

Il existe également d'autres opérateurs mathématiques utiles pour certains projets.
