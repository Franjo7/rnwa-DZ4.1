If you want to run our Laravel application, you must complete the following steps:

Import the Northwind database into MySQL: https://code.google.com/archive/p/northwindextended/downloads
Run cp .env.example .env
In .env file configure DB_DATABASE=northwind
Run composer install
Run php artisan key:generate
Run php artisan serve

Testing in Postman:

Once you open Postman, click (+) icon for creating a new request
Choose POST method and paste this url next to it: http://127.0.0.1:8000/api/customerdemographic
Go to Body, select raw and choose JSON instead of Text
Paste this block of code and click Send:
{
"CustomerTypeID": 3,
"CustomerDesc": "SomeDesc"
}

If you want to fetch all Customer Demographics, you can use GET method with the same url as above

If you want to update Customer Demographic, you can use PUT method with this url: http://127.0.0.1:8000/api/customerdemographic/3
After selecting Body and choosing JSON, paste this block of code and click Send:
{
"CustomerTypeID": 3,
"CustomerDesc": "SomeSomeSomeDesc"
}

If you want to delete Customer Demographics, you can use DELETE method with the same url as above
