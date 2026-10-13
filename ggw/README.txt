GOSAT-GW ARカメラ（説明切替・縦横対応・写真共有版）

内容:
- index.html
- ggw.glb

使い方:
1. index.html と ggw.glb を同じフォルダに置き、HTTPS対応のWebサーバーから開いてください。
2. カメラ開始を押して、ブラウザのカメラ利用を許可してください。
3. 指1本で衛星を移動、2本指で拡大・縮小できます。調整ボタンも使えます。
4. 撮影・保存で画像をダウンロードします。対応ブラウザでは「共有・写真に保存」から共有メニューを開けます。

説明文の切り替え:
- 日本語: index.html
- English: index.html?lang=en
- 子供向け日本語: index.html?lang=kids

補足:
- スマートフォンの向きに合わせて表示と撮影画像の縦横を切り替えます。
- Webページから写真ライブラリへの無確認の直接保存はできないため、共有メニューまたはダウンロードを使用します。
- カメラはHTTPS接続が必要です（localhostを除く）。
- Three.jsはCDNから読み込みます。利用時にインターネット接続が必要です。

追加修正:
- カメラ開始後に説明文を自動で折りたたみます。右上の「説明を表示」で再表示できます。
- 説明文の領域が衛星操作のタッチを遮らないようにしました。
- Android向けに screen.orientation、resize、orientationchange、visualViewport の変化を監視して画面レイアウトを更新します。

Android横向き追加修正:
- screen.orientation.type の値が古いままの場合に備え、実際の表示領域 innerWidth/innerHeight も優先して横向きを判定します。
- Android Chromeで画面サイズの更新が少し遅れる場合に備え、回転後のレイアウト更新を複数回行います。
