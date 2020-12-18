<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

## About

Laravel8を用いたECサンプルアプリ

機能
- ユーザー登録・ログイン
- メインページ()
- カートページ
- 購入ページ

## How to use

- Clone this repository into document root /usr/share/nginx/html/laravel
```
git clone https://github.com/siwai0208/food-app laravel
```

- chmod
```
chmod -R 777 storage
chmod -R 777 bootstrap/cache/
```

- Composer update
```
composer update
```

- .envファイルを編集
```
cp .env.example .env
vim .env
 DB_HOST=xxxx
 DB_DATABASE=xxxx
 DB_USERNAME=xxxx
 DB_PASSWORD=xxxx
```

- DB migrate
```
php artisan key:generate
php artisan config:cache
php artisan migrate
```

- DB seed (Option)
```
php artisan db:seed
```
