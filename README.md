# Memocca-Server

## 概要

 アカウント登録もなく、インスタントに使えるホワイトボードアプリです。
 以下のURLはデモサイトです。
 [https://stickyboards.netlify.app/](https://stickyboards.netlify.app/)

## 説明

- 付箋紙と手書き文字がかけるシンプルなホワイトボードアプリです。
- 用意してあるdocker-composeファイルを用いることで、ローカル・オンプレミス環境にセットアップ可能です。
なので、既存のサービスのように、機密情報を外部サーバーに置かれる心配がありません。
- 初回起動後に1つ、部屋が自動で作成されるので、URLを共有して、テレビ会議等ですぐに使えます。

## 使い方

```bash

$ docker-compose up -d

```

## 開発のはじめ方

1. python3.6以降をインストールします。
   1. virtualenvなどの仮想環境をオススメします。
2. プロジェクトルートで、以下のコマンドを実行して、必要なパッケージをインストールします。

   ```bash
    $ pip install -r requirements.txt
   ```

3. APIの疎通を確認したら、開発環境のセットアップは、完了です。

   ```bash
    $ python ./src/main.py
    $ curl http://localhost:8080/
   ```

## ライセンス

未定
