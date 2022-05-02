# webapp
laravel

If you see a message like the one below when you access localhost, follow step 1.
require(/var/www/html/public/../vendor/autoload.php): failed to open stream: No such file or directory in /var/www/html/public/index.php on line 34

step 1.

Run following command in app container
$ composer install

If you see a message like the one below in /storage/logs/laravel.log when you access localhost, follow step 2.
No application encryption key has been specified.

step 2.

Run following command in app container
$ cp .env example .env
$ php artisan key:generate
