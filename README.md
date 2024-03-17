# Laravel Chat Application Realtime

Aplikasi chatting realtime sederhana menggunakan laravel 11, pusher dan chatify

## Installation

```bash
  git clone https://github.com/hndko/app_laravel_chat.git
  cd app_laravel_chat
```

Terminal 1 dengan composer & artisan

```bash
  composer install
  php artisan key:generate
  cp .env.example .env
```

Edit .env

```bash
Database
Before:
  DB_CONNECTION=sqlite
  # DB_HOST=127.0.0.1
  # DB_PORT=3306
  # DB_DATABASE=laravel
  # DB_USERNAME=root
  # DB_PASSWORD=

After:
  DB_CONNECTION=mysql
  DB_HOST=127.0.0.1
  DB_PORT=3306
  DB_DATABASE=db_laravel_chat
  DB_USERNAME=root
  DB_PASSWORD=

---------------------------------------------------------
Add Pusher Config :
  PUSHER_APP_ID={Your-API-ID}
  PUSHER_APP_KEY={Your-API-KEY}
  PUSHER_APP_SECRET={Your-API-SECRET}
  PUSHER_HOST=
  PUSHER_PORT=443
  PUSHER_SCHEME=https
  PUSHER_APP_CLUSTER={Sesuaikan Dengan APP CLUSTER Pusher}
```

Lanjutan terminal 1

```bash
  php artisan migrate (option = yes)
  php artisan serve
```

Terminal 2 dengan npm

```bash
  npm install
  npm run dev
```

## Documentation

-   [Laravel](https://laravel.com/)
-   [Chatify](https://chatify.munafio.com/)
-   [Pusher](https://dashboard.pusher.com/)
