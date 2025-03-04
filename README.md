# Docker Compose Template

---

This template makes it easy to spin up a PHP 8.1 environment with docker compose.

## Laravel

In this repo there is a Laravel 10 branch. To get started with this branch run these commands

`git clone git@github.com:NicholasMartens/docker-compose-php8.1.git`

`cd docker-compose-php8.1/`

`git fetch origin laravel11-postgres`

`git checkout laravel11-postgres`

`docker compose up -d`

`docker compose exec cli composer install`

`docker compose exec cli php artisan key:generate`

`docker compose exec cli php artisan migrate`

After this there should be a Laravel project running on **port 8000**.
The `.env` file included has the credentials to the database. Change these credentials and add the `.env` file to the `.gitignore` file

### Interesting Packages

- https://filamentphp.com/
- https://laravel.com/docs/10.x/horizon
- https://laravel.com/docs/10.x/telescope
