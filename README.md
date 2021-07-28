# Cline Backend

## Description
Clineのバックエンド

## Environment
|言語、フレームワークなど|バージョン|
|:---:|:---:|
Ruby| 2.7.4
Rails| 6.1.3
MySQL| 8.0.22

## Set Up
1. イメージ作成
```
docker compose build
```

2. DBの構築
```
docker compose run --rm web rails db:create
```

3. コンテナの立ち上げ
```
docker compose up -d
```

## Usages

### dockerの停止
```
docker compose down
```

### dockerの再起動
```
docker compose restart
```

### dockerのログ確認
```
docker compose logs -f web
```

### rspecの実行
```
docker compose exec web bundle exec rspec ./spec
```
