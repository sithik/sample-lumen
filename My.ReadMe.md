
Steps to setup:

`git clone code-repo directory`
`cd directory`
`composer install`
configure `.env` for DB
`composer dump-autoload`
php artisan migrate:fresh
php artisan db:seed --class=UsersTableSeeder