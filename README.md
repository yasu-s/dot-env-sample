# 概要

dotenvを使用してNode.js実行前に設定を読み込むサンプルです。

# 実行環境

* Node.js - 10.x
* Yarn - 1.12.x

# 使用ライブラ

* dotenv - 8.1.x

# 動作確認

```
# dotenvによる読み込みなし
$ node index.js
# output: undefined

# dotenvによる.envファイル読み込み
$ node -r dotenv/config index.js
# output: hoge

# dotenvによる.env-localファイル読み込み
$ node -r dotenv/config index.js dotenv_config_path=./.env-local
# output: hogehoge
```
