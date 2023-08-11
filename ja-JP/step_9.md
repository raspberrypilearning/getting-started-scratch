## イベント

`イベント`{:class="block3events"}メニューのブロックは、スクリプトが開始されるタイミングを制御します。

**ハットブロック** は、特定のイベントが発生したときに、その下のブロックを実行します。 上部が帽子のように丸くなっているので、ほかのブロックはその上に置くことができません。

以下を使用できます。

```blocks3

when flag clicked // ステージの上の緑色の旗がクリックされたときにブロックを実行します

when this sprite clicked // このスクリプトのスプライトがクリックされたときにブロックを実行します

when stage clicked // ステージがクリックされたときにブロックを実行します

```

**ヒント:** `ステージが押されたとき`{:class="block3events"}ブロックはステージのコードエリアで作業している場合にのみ使用可能です。

キーボードを搭載したコンピューターを使用している場合は、`キーが押されたとき`{:class="block3events"}を使うことができます。

```blocks3
when [space v] key pressed // 数字、文字、または矢印キーに変更します
```

`背景が[背景1]になったとき`{:class="block3events"}ブロックを使えば、背景が変わるタイミングでスクリプトを開始することもできます。

[[[scratch3-changing-backdrops-pages-levels]]]

[[[scratch3-show-hide-sprites-backdrops]]]


`[音量] > (10)のとき`{:class="block3events"}ブロックには2つのバージョンがあります。

```blocks3
when [loudness v] > (10) // マイクが音を検出したときにブロックを実行します

when [timer v] > (10) // タイマーが10秒に達したときにブロックを実行します
```

[[[scratch3-time-delay]]]


`イベント`{:class="block3events"}メニューの最後の2ブロックは、 `メッセージ`{:class="block3events"}関連のブロックです。 `(メッセージv)を受け取ったとき`{:class="block3events"}を使って、任意のスプライトが対応する `(メッセージv)を送る`{:class="block3events"}ブロックを実行したときにスクリプトを開始することができます。

[[[generic-scratch3-broadcast-message]]]

