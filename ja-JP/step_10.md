## 制御

`制御`{:class="block3control"}ブロックは、決定(選択)やループ(繰り返し)など、ブロックが実行される順序を制御します。


`待つ`{:class="block3control"}ブロックは、次のブロックを実行するのを指定した秒数だけ遅らせます。

```blocks3
wait (1) seconds// delay for 1 second

wait (0.1) seconds// delay for one tenth of a second
```

ループは、ループ内のコードが実行される回数を制御します。

```blocks3
repeat (4) // run the blocks inside four time

end
```

```blocks3
forever // run the blocks inside until stopped

end
```

[[[scratch3-forever-condition]]]

**ヒント:** ステージの上側にある[停止]ボタンをクリックするか、 `止める`{:class="block3control"}ブロックを使用して、`ずっと`{:class="block3events"}ブロックを止めることができます。

`止める`{:class="block3events"}ブロックには、次の3つのオプションがあります。

```blocks3
stop [all v] // stop all scripts in all sprites

stop [this script v]

stop [other scripts in sprite v]
```

`もし...なら`{:class="block3control"}と`もし...なら...でなければ`{:class="block3control"}ブロックは、どのコードブロックを次に実行するか決めるのに使われます。 **選択**と呼ばれることもあります。 `もし... なら`{:class="block3control"}ブロックは、六角形の **条件**をチェックして**真**の場合、内部のコードブロックを実行します。 `もし... なら... でなければ` ブロックの場合、**偽**の場合に実行する追加のコードブロックセクションがあります。

```blocks3
if <> then

end

if <> then

else

end
```

[[[scratch3-if-then-else]]]

`演算`{:class="block3operators"}および `調べる`{:class="block3sensing"}ブロックメニューで、条件として使用する六角形のブロックを見つけることができます。

`< >まで待つl`{:class="block3control"} と `< >まで繰り返す`{:class="block3control"} ブロックも条件を使います。

```blocks3
wait until <> // delay until the condition is true


repeat until <> // repeat the blocks inside until the condtion is true

end
```

**クローン** はスプライトのコピーであり、クローン作成時にクローンされたスプライトが保持しているコスチューム、スクリプト、およびサウンドが含まれています。 スプライトのクローンを作成するために使用できるブロックは、いくつかあります。

`[自分自身v]のクローンを作る`{:class="block3control"}ブロックで、スプライトはそれ自体またはプロジェクト内の別のスプライトのクローンを作成できます。

```blocks3
create clone of [myself v] // clones the sprite that runs this block


create clone of [Butterfly 1 v] // clones another sprite in the project
```

`クローンされたとき`{;class="block3control"}ハットブロックは、クローンが作成された後、新しいスクリプトを起動するために使われます。 クローンは、`このクローンを削除する`{:class="block3control"}キャップブロックが使用されるまでプロジェクト内に存在します。

`クローンされたとき`{:class="block3control"} ハットブロックを使うとき、`[自分自身v]のクローンを作る`{:class="block3control"} ブロックをスクリプトに含めることができます。つまり、クローンがまたクローンを作ることができるということです。

```blocks3
when I start as a clone // the script that runs when the clone is created


delete this clone // stops the clone's scripts and deletes it
```

スプライトが任意の時点で持つことができるクローンの最大数が決まっています。これを書いている時点では`300`です。

--- collapse ---
---
title: クローンのクローン
---

**クローンたち**: [中を見る](https://scratch.mit.edu/projects/567544298/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567544298/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /collapse ---

