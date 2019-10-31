# Docker イメージをビルド
```
docker image build -t example/echo:latest .
```
# Docker コンテナを実行する
```
docker container run example/echo:latest
```
### バックグラウンドで実行する場合
```
docker container run -d example/echo:latest
```
### ポートフォワーディング
```
docker container run -d -p 9000:8080 example/echo:latest
```