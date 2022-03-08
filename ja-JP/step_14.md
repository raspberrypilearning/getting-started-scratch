## ブロック定義

`ブロック定義`{:class="block3myblocks"}を使用すると、スプライトの新しいブロックを作成できます。 ブロックに名前を付け、新しいブロックが、他のScratchブロックを使って何をするか`定義`{:class="block3myblocks"}します。 新しいブロックは、ブロックを所有するスプライトの任意のスクリプトで使用できます。

この例 ではスプライトのコスチュームを変える`トーク`{:class="block3myblocks"}ブロックを定義しています。

**ペンギンのさえずり**: [中を見る](https://scratch.mit.edu/projects/567554899/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567554899/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

```blocks3
define talk
switch costume to (penguin2-b v)
repeat (2)
play sound (chirp v) until done
end
switch costume to (penguin2-a v)

when this sprite clicked
talk

when [space v] key pressed
talk
```

`ブロック定義`{:class="block3myblocks"}を使用して、コード を**整理**することができます。 スプライトに話させるときに、スプライトが話すのに使うすべてのブロックをグループ化して、1つの `トーク`{:class="block3myblocks"}ブロックとして使う方が簡単です。

スプライトの話し方を変更したい場合は、コードを1か所変更するだけです。

### 入力のあるブロック定義

**入力**を `ブロック定義`{:class="block3myblocks"}に追加することができます。ブロックを使用するときに、あなたが提供した値をスプライトが使用するようになります。

**ペンギンのおしゃべり**: [中を見る](https://scratch.mit.edu/projects/567538874/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567538874/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

```blocks3
define talk (words)
switch costume to (penguin2-b v)
say (words) // use the provided input
repeat (2)
play sound (chirp v) until done
end
say (words)
switch costume to (penguin2-a v)

when this sprite clicked
talk [hello]

when [space v] key pressed
talk [hi]
```

[[[generic-scratch3-make-block]]]

--- collapse ---
---
title: ブロック定義を使用してコードを整理する
---
`ブロック定義`{:class="block3myblocks"}の最も簡単な使い方は、コードを整理することです。 これが簡単な例です。

```blocks3
define move right
if <not <touching (edge v) ?>> then
switch costume to [right_1 v]
change x by (2)
switch costume to [right_2 v]
change x by (2)
switch costume to [right_3 v]
change x by (2)
end

define move left
if <not <touching (edge v) ?>> then
switch costume to [left_1 v]
change x by (-2)
switch costume to [left_2 v]
change x by (-2)
switch costume to [left_3 v]
change x by (-2)
end

when flag clicked
forever
if <key (right arrow v) pressed> then
move right
end
if <key (left arrow v) pressed> then
move left
```

--- /collapse ---

`ブロック定義`{:class="block3myblocks"}は、他のプログラミング言語の「手続き」、「関数」、または「メソッド」に似ています。
