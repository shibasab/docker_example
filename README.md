## Docker イメージをビルド

```docker
docker image build -t example/echo:latest .
```

## Docker コンテナを実行する

```docker
docker container run example/echo:latest
```

#### バックグラウンドで実行する場合

```docker
docker container run -d example/echo:latest
```

#### ポートフォワーディング

```docker
docker container run -d -p 9000:8080 example/echo:latest
```

## イメージを検索

```docker
docker search [options] 検索キーワード
```

## イメージを取得

```docker
docker image pull [options] リポジトリ名[:タグ名]
```

## イメージの公開

```docker
docker image push [options] リポジトリ名[:タグ名]
```

## コンテナ一覧を表示

```docker
docker container ls [options]
```

## ファイルのコピー

```docker
docker container cp [options] コピー元 コピー先
```
