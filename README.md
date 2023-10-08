# MinIOとSDKでS3をテストする

```bash
docker compose build
docker compose run --rm node yarn
docker compose up -d
docker compose run --rm node node index.js
```

上記コマンドで/docker/minio/data/直下にBucketファイルが作成される。
http://localhost:9001でMinIOにログインするとBucketが存在する。


下記問いで削除可能

```bash
Empty and delete bucket? (y/n)
```
