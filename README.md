# SportsRecord UML管理リポジトリ
SportsRecordのUMLを保存

## 環境構築
### 0. Javaと[Grapviz](https://plantuml.com/ja/graphviz-dot)がインストールされていて、VScodeで開発することが前提
### 1. ルートディレクトリで以下のコマンドを実行
```
$sh plantuml_server_start.sh
```

### 2. VScodeにPlantUMLの拡張機能をインストール
拡張機能の検索窓に「jebbs.plantuml」って入れて出てくるやつ
インストールが完了したら再読み込みをする

### 3. PlantUMLのプレビューを高速にする設定をする
VScodeの設定を開き、以下の変更をする。
* 検索窓に「Plantuml:Render」と入力し、項目を「PlantUMLServer」に変更。
* 検索窓に「Plantuml:Server」と入力し、`http://localhost:8080/`を設定。

これで、VScodeでのプレビュー時に1でdockerでたてたレンダー用サーバを使うようになり、プレビューが高速になる。
プレビューはOption+Dでできる。

## 画像の保存
Shit+⌘+Pでコマンドパレットを開き、plantumlでフィルターをかけ、`PlantUML: カーソル位置のダイアグラムをエクスポート`を選択すると好きなフォーマットで保存

参考: https://qiita.com/Ping/items/64930e8c21fb95bec095