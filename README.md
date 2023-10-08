# MinIOとSDKでS3をテストする


## Usage

### 1. パッケージのインストール

```bash
docker compose run --rm node yarn
```

### 2. コンテナの起動

```bash
docker compose up -d
```

上記コマンドで`/docker/minio/data`が作成される。

この段階では[http://localhost:9001](http://localhost:9001)でMinIOコンソールにログインしてもBucketは存在しない。

| username | password |
| --- | --- |
| root | password |

### 3. index.jsファイルの実行

```bash
docker compose run --rm node node index.js
```

[http://localhost:9001](http://localhost:9001)でMinIOにログインするとBucketが存在する。


下記問いで削除可能

```bash
Empty and delete bucket? (y/n)
```
