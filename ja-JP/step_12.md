## 演算

`演算`{:class="block3operators"}ブロックは、変数と値の比較、数値による計算、および文字列（テキスト）の操作に使用されます。

六角形の「真偽値」ブロックが条件として使用され、真または偽を返します。 これらのブロックは 六角形の入力を持つ`制御`{:class="block3control"}ブロックで使用できます。

比較演算子：

```blocks3
<[] > [50]>

<[] < [50]>

<[] = [50]>
```

**ヒント:** `=`{:class="block3operators"} をテキストで使う場合、大文字と小文字を混ぜ合わせることができます。ですから、 `<`{:class="block3operators"} `YES` `=`{:class="block3operators"} `yes` `>`{:class="block3operators"} は**真**を返します。


算術演算です：

```blocks3
([] + [])

([] - [])

([] * [])

([] / [])
```

最小数と最大数（それらの数を含む）の間で乱数を選択できます。

```blocks3
(pick random [1] to [10]) // 1から10の間の数字
```

`かつ`{:class="block3operators"}、 `または`{:class="block3operators"}、および `ではない`{:class="block3operators"}演算子は、条件を結合するために使用することができます。

```blocks3
<<> and <>>

<<> or <>>

<not <> >
```

テキスト文字列を操作するためのブロックです：

```blocks3
(join [apple ] [banana])

(letter [1] of [apple])

(length of [apple])

<[apple] contains [a]>
```

[[[scratch3-join-text]]]

ほかにも、いくつかのプロジェクトで役立つ算術演算子もあります。
