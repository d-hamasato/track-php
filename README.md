## 概要
PHPでアルゴリズム問題を解く時に、デバッグできる環境が欲しかったのでDockerでつくってみた  
[すごく参考にさせてもらったサイト](https://tech-lab.sios.jp/archives/24164)

## 動作環境
vscodeで以下の拡張機能がインストール済みであること
- Remote-Containers
- Xdebug

## 使い方
- track-phpディレクトリをvscodeで開く
- ターミナルでDockerコンテナを起動 docker-compose up -d
- 左下みどりのRemote-Containersボタンをクリック
- Open Folder Container...をクリックし、Dockerコンテナに入る
- vscode左ツールバーの実行とデバッグをクリック
- 処理を止めたいところにブレイクポイントを打つ
- Listen for Xdebug 左のみどり再生ボタンをクリック
- ターミナルからphpファイルを実行 (例：php track.php)

## その他
devcontainer.json 内で設定することで、vscodeでいつも使っている拡張機能をdockerコンテナ内でも使用できる！  
PHP Intelephenseは設定済み（Xdebugも）