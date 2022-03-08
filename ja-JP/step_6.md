## 動き

`動き`{:class="block3motion"}ブロックを使用すると、スプライトをステージ内で移動させることができます。

### 移動

`(10)歩動かす`{:class="block3motion"}ブロックは、まずスプライトを移動させてみる最も簡単な方法です。

```blocks3
move [10] steps
```

マウスポインタの示す(タブレットの場合は指を置いた)ステージ上のランダムな位置や、他のスプライトの位置に `行く`{:class="block3motion"} ことや `(1)秒で行く`{:class="block3motion"}ことができます。

```blocks3
go to (random position v)

glide [1] secs to (random position v)
```

`x`{:class="block3motion"} 座標と `y`{:class="block3motion"} 座標で指定したステージ上の位置に`行く`{:class="block3motion"} ことや `(1)秒で行く`{:class="block3motion"}こともできます。

```blocks3
go to x: [0] y: [0] 

glide [1] secs to x: [0] y: [0]
```

[[[scratch3-glide-to-object]]]

**ヒント：**ステージ上のスプライトをドラッグすると、 `動き`{:class="block3motion"}ブロックメニューの`x`{:class="block3motion"} 座標と `y`{:class="block3motion"} 座標を使うブロックの座標も更新されます。 現在の `x`{:class="block3motion"} 座標と `y`{:class="block3motion"} 座標はスプライトペインに表示されます。

### 回転
スプライトが指している`方向`{:class="block3motion"}を変更することもできます。 `move`{:class="block3motion"}ブロックを使用した場合に、スプライトが移動する方向が変わります。 また、 `回転方向`{:class="block3motion"} の設定に応じてスプライトのコスチュームの向きも変えます。

スプライトを追加すると、右向き（90度）になります。 これは、スプライトペインまたはコードブロックを使用して変更できます。

```blocks3
turn right [15] degrees

turn left [15] degrees

point in direction [90] // Click on 90 and drag the arrow to change

point towards (mouse-pointer v)

(direction)

set rotation style [left-right v] // or all-around or none
```

[[[scratch3-sprite-direction]]]

[[[scratch3-left-right-direction]]]

--- collapse ---
---
title: 回転する
---

--- no-print ---

**まわるコウモリ**: [中を見る](https://scratch.mit.edu/projects/435704980/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435704980/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

このコードは、緑色の旗がクリックされたときにスプライトを回転させます。

```blocks3
when flag clicked
forever
turn right (1) degrees :: motion
```

`ずっと`{:class="block3control"}ループの `(15)度回す`{:class="block3motion"}ブロックで、 角度の数字を`1` に変更すると、スプライトが回転しているように見えます。

**ヒント:** `動かす`{:class="block3motion"}ブロックを追加しない場合、スプライトは現在の位置で回転します。

--- /collapse ---

--- collapse ---
---
title: 円を描くように動く
---

--- no-print ---

**月の軌道**: [中を見る](https://scratch.mit.edu/projects/435701055/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435701055/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

このコードは、緑色の旗がクリックされたときにスプライトを円を描くように飛ばせます。

```blocks3
when green flag clicked
forever
move (1) steps
turn right (1) degrees :: motion
```

`ずっと`{:class="block3control"}ループの `動かす`{:class="block3motion"}ブロックと `回す`{class="block3motion"}ブロックの値を`1`に変えてみましょう。スプライトは大きな円を描いて移動しているように見えます。

**ヒント:** スプライトを常にステージの中央から開始するには、 `x座標を`{:class="block3motion"} `0` `、y座標を`{:class="block3motion "} `0` `にする`{:class="block3motion"}ブロックを <1>ずっと</1>{:class=" block3control "}ブロックの前に追加します。

--- /collapse ---

### 跳ね返る

`もし端に着いたら、跳ね返る`{:class="block3motion"}ブロックは、スプライトを跳ね返らせてステージにとどまらせたい場合に非常に便利です。

```blocks3
if on edge, bounce
```

スプライトを跳ね返らせる方法のいくつかをご覧ください。

--- collapse ---
---
title: ステージを横切って跳ね返る
---

--- no-print ---

**ステージを横切って移動する女の子**: [中を見る](https://scratch.mit.edu/projects/433535326/editor){:target="_ blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433535326/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

このコードは、ステージの左端と右端でスプライトを跳ね返らせます。 スプライトは水平方向に回転するため、緑色の旗をクリックしたときに方向を変えると、スプライトが反転しているように見えます。

```blocks3
when green flag clicked
point in direction (90)
set rotation style [left-right v]
forever
move (5) steps
if on edge, bounce
```

この例では、緑色のフラグがクリックされると、 `(90)度に向ける`{:class="block3motion"}ブロックにより自動的にスプライトは右向き(`90`度)になります。 度の数を `-90`に変更した場合、スプライトは左向きになります。

`回転方法を[左右のみ]にする`{:class="block3motion"}ブロックを追加し、 ドロップダウンメニューで`左右のみ`{:class="block3motion"}を選択すると、スプライトがステージの端で跳ね返るときに上下逆さまになりません。

**ヒント:** ステージ上でスプライトをドラッグして、目的のy（上下）位置に移動できます。

--- /collapse ---

--- collapse ---
---
title: ステージの上下で跳ね返る
---

--- no-print ---

**ジャンプする女の子**:[中を見る](https://scratch.mit.edu/projects/433595822/editor){:target="_ blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433595822/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

このコードは、緑色の旗がクリックされたときにスプライトをステージの上下で跳ね返らせます。

```blocks3
when green flag clicked
point in direction (0)
set rotation style [don't rotate v]
forever
move (5) steps
if on edge, bounce
```

`(90)度に向ける`{:class="block3motion"}ブロックの度の数を `0` にするとスプライトは上向きになります。

`回転方法を[左右のみ]にする`{:class="block3motion"}ブロックを追加し、ドロップダウンメニュ0で `回転しない`{:class="block3motion"}を選択すると、スプライトが跳ね返っても回転しないようになります。

**ヒント:** スプライトをステージ中にドラッグして、目的のx（左右）の位置に移動できます。

--- /collapse ---

--- collapse ---
---
title: 斜めに跳ね返る
---

--- no-print ---

**跳ね返るサッカーボール**: [中を見る](https://scratch.mit.edu/projects/433536479/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433536479/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

このコードは、緑色の旗がクリックされたときにスプライトがランダムに回転しているように見せます。

```blocks3
when green flag clicked
point in direction (45)
set rotation style [all around v]
forever
move (5) steps
if on edge, bounce
```

スプライトを `45` 度の角度で移動させて場合、ステージの端である角度で跳ね返るように見えることがわかります。 `(90)度に向ける`{:class="block3motion"}ブロックの度の数を `45` にするとスプライトは四方八方に跳ね返ります。

`回転方法を[左右のみ]にする`{:class="block3motion"}ブロックを追加し、 ドロップダウンメニューで`自由に回転`{:class="block3motion"}を選択すると、スプライトがステージの端で跳ね返るとき回転するようになります。

--- /collapse ---

### 座標を使用する

`x座標`{:class="block3motion"} と `y座標`{:class="block3motion"を`(0)にする`{:class="block3motion"}ことや、 `(10)ずつ変える`{:class="block3motion"}こともでき、他のブロックて使うために値を取得することもできます。

[[[generic-scratch3-coordinates]]]

```blocks3 
change x by [10]

set x to [0]

change y by  [10]

set y to [0]

(x position)

(y position)
```

--- collapse ---
---
title: 動きブロックが表示されません
---

ステージを選択している場合 `動き`{:class="block3motion"}ブロックは表示されません。ステージは動くことができないからです。

スプライトペインでスプライトをクリックし、[**コード**]タブをクリックすると `動き`{:class="block3motion"}ブロックが表示されます。

--- /collapse ---

