## 調べる

`調べる`{:class= block3sensing"}ブロックメニューのブロックは、ユーザーテキスト入力を取得し、状態を検出し、プロジェクトの値として伝えます。

`制御`{:class="block3control"}ブロックのなかで、ブロックがいつ動くかの決定や制御に使う六角形の`調べる`{:class="block3sensing"} ブロックがいくつかあります。

`触れた`{:class="block3sensing"}ブロックは、スクリプトが書かれているスプライトが、マウスポインター(タブレットでは最後に指で触れた場所)、ステージの端、または別のスプライトに触れているかどうかを選んで検出することができます。

```blocks3
<touching (mouse-pointer v) ?>

<touching (edge v) ?>

<touching (Sprite2 v) ?>
```

スクリプトが書かれているスプライトが別の色(ステージまたは別のスプライト) に触れているかどうか、またはこのスプライトの色が別の色に触れているかどうかを検出するためのブロックがあります。

```blocks3
<touching color (#c5a97b) ?>

<color (#c219ed) is touching (#62d1e0) ?>
```

`キーが押された`{:class="block3sensing"}ブロックでは、キーを数字、文字、および矢印キーから選ぶことができます。 キーを入力するにはキーボードが必要です。 キーが現在押されているかどうかを検出します。

```blocks3
<key (space v) pressed?>
```

`マウスが押された`{:class="block3sensing"}ブロックは、マウスが現在押されているか、タッチスクリーンでは画面がタップまたはタッチされているかを検出します。

```blocks3
<mouse down?>
```

`聞いて待つ`{:class="block3sensing"}と `答え`{：class = "block3sensing"}ブロックは、ユーザーからのテキスト入力を取得するために使用されます。

```blocks3
ask [What's your name] and wait

(answer) // the text the the user typed 
```

`聞いて待つ`{:class="block3sensing"}ブロックは、キーボードまたはタブレットの仮想オンスクリーンキーボードで機能します。

`答え`{:class="block3sensing"}ブロックは、値を報告し、変数として使用できるレポーターブロックです。

[[[scratch3-ask-answer-chat]]]

`調べる`{:class="block3sensing"}ブロックメニューには、値を取得するために使用できるいくつかのレポーターブロックも含まれています。

```blocks3
(distance to (mouse-pointer v))

(distance to (Sprite2 v))
```

マウスポインタの現在の位置(またはタブレット上の指の現在または最新の位置) を検出できます。

```blocks3
(mouse x)

(mouse y)
```

マイクからの音の`音量`{:class="block3sensing"}を検出することができます。 ポップアップウィンドウがユーザーにマイクの使用許可を求めます。

```blocks3
(loudness)
```

`タイマー`{:class="block3sensing"} はプロジェクトが読み込まれた時にカウントし始め、`タイマーをリセット`{:class="block3sensing"}で`0`に戻すことができます。

```blocks3
(timer)

reset timer
```

ステージやその他のスプライトのレポーターにアクセスすることもできます。

```blocks3
([backdrop # v] of (_stage_ v))

([x position v] of (Sprite2 v))

([costume # v] of (Sprite2 v))
```

あなたのローカルタイムゾーンで、現実の世界の日付と時刻に関連するレポーターがあります。

```blocks3
(current [year v]) // hour, minute, ...

(days since 2000)
```

