laraveltest
====

laravelサンプル

# Install

```sh
$ git clone git@github.com:togana/laraveltest.git
```

# Usage

```sh
# ディレクトリ移動
$ cd laradock
# 環境構築
$ docker-compose up -d --build nginx php-fpm mysql workspace
# ワークスペース
$ docker-compose exec workspace bash
# パッケージインストール
$ composer install
# マイグレーション
$ php artisan migrate
# データ挿入
$ php artisan tinker
Psy Shell v0.8.1 (PHP 7.0.14-2+deb.sury.org~xenial+1 — cli) by Justin Hileman
>>> $posts = new App\Post();
=> App\Post {#643}
>>> $posts->title = 'title 1';
=> "title 1"
>>> $posts->content = 'content1';
=> "content1"
>>> $posts->save();
=> true
```



