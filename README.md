# reviewManager

コードレビューの指摘をサイドバーにまとめ、修正したものを Cursor の Agent に渡す拡張です。

このリポジトリには配布用のパッケージだけを置いています。

## インストール

1. [Releases](https://github.com/shion555/reviewmanager/releases) から `reviewmanager-0.0.1.vsix` をダウンロードします。
2. Cursor の拡張機能ビューで **Install from VSIX...** を選び、そのファイルを指定します。
3. ウィンドウを再読み込みします。左のアクティビティバーに reviewManager が出ます。

## 使い方

1. 設定の `reviewmanager.prompt` に、レビューの依頼文を書きます。
2. サイドバーの **レビューを依頼** を押します。依頼文が Agent の入力欄に入ります。
3. Agent が `.reviewmanager/findings.json` に指摘を書くと、サイドバーに **High**、**Middle**、**Low** の順で表示されます。
4. 直した指摘にチェックを入れ、**選択した修正を送る** を押します。選んだ指摘が Agent の入力欄に入ります。

送信は Agent 側で行います。
