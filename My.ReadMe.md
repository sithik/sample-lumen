
# Steps to setup


`git clone code-repo directory`

`cd directory`

`composer install`

configure `.env` for DB

    DB_CONNECTION=pgsql
    DB_HOST=localhost
    DB_PORT=5432
    DB_DATABASE=sample
    DB_USERNAME=postgres
    DB_PASSWORD=postgres



`composer dump-autoload`

`php artisan migrate:fresh`

`php artisan db:seed --class=UsersTableSeeder`



`php -S localhost:8000 -t public`


`curl http://localhost:8000/users/1` or `http://localhost:8000/users/1` in Postman on Browser to get data
