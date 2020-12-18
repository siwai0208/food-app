<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

## About

Laravel8を用いたECサンプルアプリ

機能
- ユーザー登録・ログイン
- メインページ (15アイテム表示)
- カートページ
- 購入ページ

## How to use

1. LEMPインフラの準備
  <br>[Docker LEMP環境構築](https://github.com/siwai0208/docker-template)

2. Clone this repository into document root (/usr/share/nginx/html/laravel)
```
git clone https://github.com/siwai0208/food-app laravel
```

3. storage と　bootstrap/cache/　のパーミッション変更
```
chmod -R 777 storage
chmod -R 777 bootstrap/cache/
```

4. Composer update
```
composer update
```

5. .envファイルを編集
```
cp .env.example .env
vim .env
 DB_HOST=xxxx
 DB_DATABASE=xxxx
 DB_USERNAME=xxxx
 DB_PASSWORD=xxxx
```

6. DB migrate
```
php artisan key:generate
php artisan config:cache
php artisan migrate
```

7. DB seed to update item (Option)　
```
php artisan db:seed
```
