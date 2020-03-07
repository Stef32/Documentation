[Return to main page](README.md)

----

# 出力テストのテストグリッドを作る

15x15mmの四角を作ります。スピードを最も遅い速度に設定して、パワーは100%にセットします。(i.e. もし出力過多にならない出力値が70%の場合、70%にセットする)。

先ず、先程作った四角を並べられるだけ並べていきます。今回は10個並べることにしましょう。

次に一番左の四角を選択してプロパティーのタブを開きます。そして一番低い出力値に設定します - 上で行った作業と同じにして、今回は10%にします。 ここで設定した10%は上でセットした70%の中の10%になります。

それぞれの四角を指定していって、徐々にその出力を上げていきます - 今回のケースでは10%ずつ。

これで難しい設定は完了です！次に全ての四角を選択してからGrid toolを使ってもうワンセットの四角の列を作ります。

新しく作った四角の列を選択してから、今度は先程の列より少しだけ早くした設定にします。出力値自体は最初に作ったセットと同じにすることを忘れないでください。

LightBurn は出力比率は記憶しているので、スピードと出力の設定だけを行ってください。

この設定によってX軸は出力のY軸ではスピードのテスト結果を確認することが出来ます。


**DSPユーザーの注意点:**

もしRuidaかその他DSP controllerを利用しているのであれば, 最大と最小の出力値を設定する際に、最小値はしっかりとTubeに出力が出来る値に設定してください。全てのTubeは少しずつ出火のポイントが異なっていて、今回の例として10%としてみましょう。もしあなたの最小の設定が10%で最大が80%ならば、出力のパラーメーターはその間の値を使うことになっています。もしスケールが0%ならば、最小値(10%)を使えということになります。もしスケールが50%ならば、最小と最大の真ん中を出力(10と80の間なので45%)、100%の場合は最大値なので80%ということになります。テスト時にはちょっと分かりにくいですが、それでもテストグリッドを作るには非常に有効な設定です。
