## デバッグ

**デバッグ** とは**バグ**と呼ばれるコード内の間違いを見つけて修正することです。

* 一度に1つの変更を加えてからプログラムを実行すると、問題を特定しやすくなります。

* プロジェクトが計画どおりに機能するには、実験を何度か行うことが必要になる場合があります

プロジェクトが目的の動作をしていないときにプロジェクトをデバッグするのに役立つヒントを次に示します。

--- collapse ---
---
title: コードの小さな部分だけを実行する
---

追加した最後のいくつかの新しいブロックが機能するかどうかを確認するために、プログラム全体を実行する必要はありません。

* コードエリアでブロックをクリックして実行します—ブロックが期待どおりに機能していることを確認する簡単な方法です

* ブロックのセットを単独でテストするには、**ブロックを含む ** スクリプトからブロックをドラッグし、クリックしてテストしてから、元のスクリプトにドラッグして戻します。

--- /collapse ---

--- collapse ---
---
title: 遅延を一時的に追加する
---

あなたのコードを動かすときに **実行** 速度を遅くします。 これを行うには、 `待つ`{:class="block3control"}または `キーが押されるまで待つ`{:class="block3control"}ブロックを追加し、コードのデバッグが終了したらブロックを削除します。

--- /collapse ---

--- collapse ---
---
title: ステージに変数を表示する
---

プロジェクトで `変数`{:class="block3variables"}を使ってデータを保存している場合は、`変数`{:class="block3variables"}をステージに表示すると便利です。

`変数`{:class="block3variables"}ブロックメニューの`変数`{:class="block3variables"}の横にあるチェックボックスをクリックして、ステージ上で表示または非表示にします。

変数は常に思い通りの値になっていますか？

--- /collapse ---

--- collapse ---
---
title: コメントを追加する
---

ブロック、ブロックのセット、および/またはスクリプトにコメントを追加します。 日常の言葉を使って、コードの機能を説明します。 コメントを書くことで、コードが実際にあなたがしたいことをしていないことに気付くことがあるでしょう！

コメントは、後でコードを理解したいときに役立ち、他の人があなたのプロジェクトを理解するのに役立ちます。

--- /collapse ---


多くの初心者(そして専門家も！) がScratchで経験する一般的な問題があります。

--- collapse ---
---
title: 特定の問題のデバッグのヒント
---

+ **私のスプライトが上下逆になっています** ー `回転方法を左右のみにする`{:class="block3motion"}または `設定方法を回転しないにする`{:class="block3motion"}ブロックを追加します。

+ **コスチュームを変更するときや、跳ね返るとき、スプライトが「ジャンプ」します** —コスチュームがペイントエディタの中央にあることを確認します(コスチュームの青い十字をペイントエディタの中央にある十字線に合わせます)。

+ **スプライトがステージの端まで行くと停止します**ー `もし端に着いたら、跳ね返る`{:class="block3motion"}ブロックを追加します。

+ **サウンドが再生されません** ー スプライトがクリックされたときに`音を鳴らす`{:class="block3sound"}ブロックを追加しましたか？ 別のスプライトからコードをコピーした場合は、 **音** タブでこのスプライトに音を追加する必要があります。 パソコンやタブレットのボリュームをチェックしてください、また、コードで音量を下げていないことを確認してください。 － `音量を・・・%にする`{:class="block3sound"}ブロックを`100`にしてみてください。

+ **他のスプライトが私のスプライトの前を移動します** ー `最前面へ移動する`{:class="block3looks"}ブロックを使ってみてください。

+ **スプライトが1回だけしか移動/変化しません** — コードを `ずっと`{:class="block3control"} ブロック内に配置して、実行を継続します。

+ **可変スライダーを動かしてもスプライトが変わりません** ー `ずっと`{:class="block3control"} ブロック内に配置して、更新を継続します。

--- /collapse ---

**ヒント:** これらの手法を試しても問題が見つからない場合は、休憩するか、プロジェクトの別の部分の作業をしてみてください。 戻ってきたら、すぐにバグを見つけるかもしれません！
