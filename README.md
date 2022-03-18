# Laravelを使って認証機能を実装

## 使用バージョン

- PHP v8.1.3
- Laravel v8.83.5
- MySQL v5.7.37

## プロジェクトのセットアップ手順

ターミナルでgit cloneして作成されたフォルダに移動して、下記のコマンドを実行してください。

- このプロジェクトで使用するライブラリをインストール

```bash
$ composer install
```

- .env.exampleを.envにリネームして、DBの設定を行います
- DBはMySQLを使っているのでMySQLにDBを作ります

- アプリケーションキーの初期化を行います。(ユーザーのセッション情報、パスワードの暗号化をよりセキュアにすることができます。)

```
$ php artisan key:generate
```

- テーブルの作成をします。

```bash
$ php artisan migrate
```

- サーバーを起動します。

```bash
$ php artisan serve
```

- 以上のコマンドが正しく実行できた場合、ブラウザで`localhost:8000`にアクセスします。
- ユーザーの新規登録、ログインができるか確認します。
