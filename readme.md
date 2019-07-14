# Laravel Authentication with Passport
## How do I set this up?

### Clone the repo to your local machine

```html
git clone git@github.com:chidang/laravel-passport.git
cd path-to-project/laravel-passport
composer install
```
![Clone](https://github.com/chidang/laravel-passport/blob/master/public/media/command-1.png "Clone")

### Copy file .env.example to .env

```html
cp .env.example .env
```

### Create database and update your .env file

```html
DB_CONNECTION=mysql
DB_HOST=localhost
DB_PORT=3306
DB_DATABASE=laravel-passport
DB_USERNAME=root
DB_PASSWORD=
```
### Running Migrations

```html
php artisan migrate
```
![migrate](https://github.com/chidang/laravel-passport/blob/master/public/media/command-migrate.png "migrate")

### Install passport

```html
php artisan passport:install
```

We will now test that everything is ok with Postman (you can use any other tool to simulate http requests).

Postman collection:
https://github.com/chidang/laravel-passport/blob/master/laravel-passport.postman_collection.json

![register](https://github.com/chidang/laravel-passport/blob/master/public/media/api-register.png "Register")
![login](https://github.com/chidang/laravel-passport/blob/master/public/media/api-login.png "Login")
![current-user](https://github.com/chidang/laravel-passport/blob/master/public/media/api-current-user.png "Current user")


