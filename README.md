# Benedu

## Introduction
自由な空間で学びたい学生たち

## To build
- Create a database locally named `benedu`
- Download composer https://getcomposer.org/download/
- Pull Laravel/php project from git provider.
- Rename `.env.example` file to `.env`inside your project root and fill the database information.
  (windows wont let you do it, so you have to open your console cd your project root directory and run `mv .env.example .env` )
- Open the console and cd your project root directory
- Run `composer install` or ```php composer.phar install```
- Run `php artisan key:generate` 
- Run `php artisan migrate`
- Run `php artisan db:seed` to run seeders, if any.
- If you get an error when you're using seed, like "Cannot write to directory public/storage/", please delete storage folder and run `php artisan storage:link`
- Run `php artisan serve`

#####You can now access your project at localhost:8000 :)

## If for some reason your project stop working do these:
- `composer install`
- `php artisan migrate`