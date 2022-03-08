## イベント

`イベント`{:class="block3events"}メニューのブロックは、スクリプトが開始されるタイミングを制御します。

**ハットブロック** は、特定のイベントが発生したときに、その下のブロックを実行します。 上部が帽子のように丸くなっているので、ほかのブロックはその上に置くことができません。

以下を使用できます。

```blocks3

when flag clicked // run blocks when the green flag above the Stage is clicked

when this sprite clicked // run the blocks when the sprite for this script is clicked

when stage clicked // run the blocks when the stage is clicked

```

**ヒント:** `ステージが押されたとき`{:class="block3events"}ブロックはステージのコードエリアで作業している場合にのみ使用可能です。

キーボードを搭載したコンピューターを使用している場合は、`キーが押されたとき`{:class="block3events"}を使うことができます。

```blocks3
when [space v] key pressed // change to number, letter or arrow keys
```

`背景が[背景1]になったとき`{:class="block3events"}ブロックを使えば、背景が変わるタイミングでスクリプトを開始することもできます。

[[[scratch3-changing-backdrops-pages-levels]]]

[[[scratch3-show-hide-sprites-backdrops]]]


`[音量] > (10)のとき`{:class="block3events"}ブロックには2つのバージョンがあります。

```blocks3
when [loudness v] > (10) // run blocks when the microphone detects sound

when [timer v] > (10) // run blocks when the timer reaches 10 seconds
```

[[[scratch3-time-delay]]]


`イベント`{:class="block3events"}メニューの最後の2ブロックは、 `メッセージ`{:class="block3events"}関連のブロックです。 `(メッセージv)を受け取ったとき`{:class="block3events"}を使って、任意のスプライトが対応する `(メッセージv)を送る`{:class="block3events"}ブロックを実行したときにスクリプトを開始することができます。

[[[generic-scratch3-broadcast-message]]]

