# NodeGoat

### Nodeのバージョン
デフォルトでは8系にしていますが、Dockerfileの修正でバージョンを切り替えられます。  
ただし、docker buildからやり直す必要があります。  
```yaml
FROM node:8
FROM node:8-alpine
```
バージョンは下記リンクから確認できます。
https://hub.docker.com/_/node/

### エージェントのDL
Nodejs用のエージェントをDLして、ダミーファイルと入れ替えてください。

### contrast_security.yamlのDL
定義ファイルをDLして、ダミーファイルと入れ替えてください。
アプリ名、サーバ名の設定などは任意で。

### ビルドと起動
```
docker-compose build --no-cache
docker-compose up -d
```

### NodeGoatに接続する。
http://localhost:4000/

## License
Code licensed under the [Apache License v2.0.](http://www.apache.org/licenses/LICENSE-2.0)
