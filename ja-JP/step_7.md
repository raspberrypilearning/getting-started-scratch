## 見た目

`見た目`{:class="block3looks"}ブロックは、ステージでのスプライトの外観を制御します。

スプライトは、 `言う`{:class="block3looks"}吹き出しや、 `考える`{:class="block3looks"}吹き出し、または `グラフィック効果`{:class="block3looks"}など、 `見た目`{:class="block3looks"}ブロックを使ってコミュニケーションをすることができます。

### 言うと考える

```blocks3
say () for () seconds

say ()

think () for () seconds

think ()
```

--- collapse ---
---
title: 吹き出しを使用してコミュニケーションする
---

スプライトは `言う`{:class="block3looks"} ことや `考える`{:class="block3looks"} ことでコミュニケーションします。

The `() と () 秒言う`{:class="block3looks"} と `() と () 秒考える`{:class="block3looks"} ブロックは設定した時間何かを言ったり考えたりするのに使われます。

```blocks3
when this sprite clicked
say [こんにちは] for [2] seconds // 2秒後に言葉を非表示にする
```

スプライトをクリックすると、吹き出しが2秒間表示されます。

**宇宙でおしゃべり**: [中を見る](https://scratch.mit.edu/projects/606912139/editor){:target="_blank"}

スプライトをクリックすると、話したり考えたりしてコミュニケーションします。

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/606912139/?autostart=false" frameborder="0"></iframe>
</div>

`()と言う`{:class="block3looks"}および `()と考える`{:class="block3looks"}ブロックは、何を言ったり考えるたりするときに使用され、別のメッセージまたは空の`()と言う`{:class="block3looks"}や `()と考える`{:class="block3looks"}ブロックがそれを置き換えます。

--- /collapse ---

### 大きさ

スプライトの`大きさ`{:class="block3looks"}を設定または変更します。

```blocks3
change size by ()

set size to () %

(size)
```

--- collapse ---
---
title: スプライトの大きさを設定する
---

プロジェクトにスプライトを追加したとき、大きさは`100` ％に設定されています。 そのプロジェクトで使用するには、大きすぎるたり小さすぎたりするかもしれません。

コードを使用して、スプライトの大きさを設定できます。 これを行うには、 `大きさを(100)%にする`{:class="block3looks"}ブロックを使用します。

```blocks3
set size to (50) %
```

スプライトの大きさを`50` ％に設定した場合 、半分の高さで半分の幅になります。 スプライトの大きさを`200` ％に設定した場合 、2倍の高さで2倍の幅になります。

プロジェクトが開始されたときにスプライトの大きさを設定するには、 `大きさを(100)%にする`:{class="block3looks"}ブロックを `緑色のフラグが押されたとき`{:class="block3events"}ブロックの下に置きます。

```blocks3
when green flag clicked
set size to (50) %
```

ステージの下の[スプライト] ペインの **大きさ** プロパティで、スプライトの大きさをすばやく設定することもできます。

![スプライトペインで強調表示されている[大きさ] ボックス](images/spriteSize.png){:width="400px"}

--- /collapse ---

### 画像効果

色、魚眼レンズ、渦巻き、ピクセル化、モザイク、明るさ、幽霊など、さまざまな視覚効果を設定または変更します。

```blocks3
change [色 v] effect by ()

set [色 v] effect to ()

clear graphic effects
```

[[[scratch3-graphic-effects]]]

### コスチューム

スプライトでアニメーション効果を出すには、スプライトのコスチュームを変更します。

```blocks3
コスチュームを（v）にする

次のコスチュームにする

（コスチュームの[番号v]）
```

[[[scratch3-change-costumes-to-show-mood]]]

--- collapse ---
---
title: アニメーション効果を出すために外観を変更する
---

**ドキドキする心臓**: [中を見る](https://scratch.mit.edu/projects/435725413/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/435725413/?autostart=false" frameborder="0"></iframe>
</div>

`大きさを(100)%にする`{:class="block3looks"}ブロックまたは、 `大きさを(10)ずつ変える`{:class="block3looks"}ブロック使用して、心臓の鼓動のような脈打つ効果を出すことができます。

**注:** `大きさを(100)%にする`{:class="block3looks"}ブロックは大きさを特定の値に設定し、 `大きさを(10)ずつ変える`{:class="block3looks"}ブロックは値を元の値から変更します。例えば `大きさを{:class="block3looks"} <code>10` <1>ずつ変える</code>{:class="block3looks"}ブロックは大きさの値に10を加算します。

```blocks3
when green flag clicked
set size to (160) %
forever
change size by (40)
wait (0.2) seconds
change size by (20)
wait (0.2) seconds
change size by (-20)
wait (0.2) seconds
change size by (-40)
wait (0.2) seconds
end
```

このコードは、一連の `大きさを(10)ずつ変える`{:class="block3looks"}と `<>まで待つ`{:class="block3control"}ブロックを使用して、心臓を大きくしたり小さくしたりします。 あなたの脈打つスプライトを作成してみてください。

`(色)の効果を(25)ずつ変える`{:class="block3looks"}ブロックを使用して、外観を変更し続けるスプライトを作成することもできます。

```blocks3
when green flag clicked
change [幽霊 v] effect by (75)
wait (1) seconds
change [幽霊 v] effect by (-75)
```

**注:**もしグラフィック効果を変更し、そして再びそれを変更するコードを使用するならば、`グラフィック効果を変更する`{:class="block3looks"} ブロックの間に `待つ`{:class="block3control"} ブロックを使うことを忘れないでください、そうしないと、非常に高速に変更されるため、見ることができません。

`画像効果をなくす`{:class="block3looks"}ブロックを使えば、いつでも効果をなくすことができます。

```blocks3
clear graphic effects
```

--- /collapse ---

--- collapse ---
---
title: クリックすると変化してから元に戻る
---

スプライトが大きくなって、しばらく待って、小さくなるというように、変化してしてから元に戻るアクションを追加ことができます。

**クリックしてボールを押しつぶす**: [中を見る](https://scratch.mit.edu/projects/435723273/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435723273/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

このコードは、 スプライトを大きくし、`魚眼レンズ`{:class="block3looks"}効果を0.5秒間適用してから、スプライトを最初の外観に戻します。

```blocks3
when this sprite clicked
set size to (110)
set [魚眼レンズ v] effect to (50)
wait (0.5) seconds
set [魚眼レンズ v] effect to (0)
set size to (100)
```

--- /collapse ---

[[[scratch3-animate-movement-costumes]]]

### 背景

コードを使用して背景を変更することもできます。

```blocks3
switch backdrop to ( v)

next backdrop

(backdrop [番号 v])
```

[[[scratch3-changing-backdrops-pages-levels]]]

### 見え方

`表示する`{:class="block3looks"}ブロックと `隠す`{:class="block3looks"}ブロックはスプライトの見え方を制御します。

```blocks3
show 

hide
```

[[[scratch3-show-hide-sprites-backdrops]]]

### 層

スプライトの見え方の相互関係を変更するには、層を使用します。

```blocks3
go to [front v] layer

go [forward v] () layers
```

[[[scratch3-positioning-with-layers]]]

--- collapse ---
---
title: スプライトを多くの層に配置する
---

**木の見える窓を介して**: [中を見る](https://scratch.mit.edu/projects/454188775/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe allowtransparency="true" width="485" height="402" src="https://scratch.mit.edu/projects/embed/454188775/?autostart=false" frameborder="0"></iframe>
</div>

例では、 **窓枠** スプライトが前面に表示され、 **太陽**スプライトが 背面に表示されます。 **Avery Walking** および **Tree** スプライトは**窓枠** スプライトと **太陽** スプライトの間の独自の層にあります。

`1``層奥に下げる`{:class="block3looks"} ブロックを使って前にあるスプライトより1層後ろの層に配置します。

``` blocks3
when green flag clicked
go to [front v] layer
+go [backward v] (1) layers
```

他のスプライトに対してどの位置に置くかに応じて、各スプライトの`1``層奥に下げる`{:class="block3looks"} ブロックの値を変更します。

``` blocks3
when green flag clicked
go to [front v] layer
+go [backward v] (2) layers
```

--- /collapse ---

