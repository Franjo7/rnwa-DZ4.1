If you want to run our Laravel application, you must complete the following steps:

1. Import the Northwind database into MySQL: https://code.google.com/archive/p/northwindextended/downloads
2. Run cp .env.example .env
3. In .env file configure DB_DATABASE=northwind
4. Run composer install
5. Run php artisan key:generate
6. Run php artisan serve

If you want to test REST API interface, you should check "Postman instructions.pdf".


Testing test account in Postman:

username:test-user
email:test@gmail.com
password:test1234
Authorization->Type->Basic Auth



