# web-portfolio-yumi

このプロジェクトは、練習用ポートフォリオのソースコードです。

## コンテナ起動

プロジェクトルートで以下のコマンドを実行

```sh
docker run -dit --rm --name portfolio1 -v "$PWD/public":/usr/local/apache2/htdocs/ -p 3000:80 httpd:2.4-alpine
```

## アクセス

コンテナ起動中は、以下の URL にアクセス

<http://localhost:3000/>

## コンテナ終了

終了時は以下のコマンドでコンテナを終了
（※ `docker run` コマンドで --rm を使用している場合は Ctrl + C でプロセスを終了すると、自動的にコンテナも削除される。）

```sh
docker stop portfolio1
```
## WebページURL
https://web-portfolio-sample-shirai.herokuapp.com/
