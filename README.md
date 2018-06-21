# lerna-sandbox
lerna-sandbox

lernaのテスト用リポジトリ

# インストール
`npm install -g lerna`

# npm install相当の初期化(node_modulesを削除)
`lerna bootstrap`

# クリーン(node_modulesを削除)
`lerna clean`

# 特定の子パッケージのみにパッケージを追加
ex) sub1にreduxを追加
`lerna add redux --scope=sub1-name`

なお、このコマンドはプロジェクトルートにインストールしたlernaを`npm run`で叩くとうまくいかない。
(上記の例だと、main1とmain2にもreduxがインストールされてしまう)
