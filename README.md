If you want to run our Laravel application, you must complete the following steps:

1. Import the Northwind database into MySQL: https://code.google.com/archive/p/northwindextended/downloads
2. Run cp .env.example .env
3. In .env file configure DB_DATABASE=northwind
4. Run composer install
5. Run php artisan key:generate
6. Run php artisan serve

Testing in Postman:

1. Once you open Postman, click (+) icon for creating a new request.   
2. Choose POST method and paste this url next to it: http://127.0.0.1:8000/api/customerdemographic
3. Go to Body, select raw and choose JSON instead of Text
4. Paste this block of code and click Send:
{
"CustomerTypeID": 3,
"CustomerDesc": "SomeDesc"
}

1. If you want to fetch all Customer Demographics, you can use GET method with the same url as above

1. If you want to update Customer Demographic, you can use PUT method with this url: http://127.0.0.1:8000/api/customerdemographic/3
2. After selecting Body and choosing JSON, paste this block of code and click Send:
{
"CustomerTypeID": 3,
"CustomerDesc": "SomeSomeSomeDesc"
}

1. If you want to delete Customer Demographics, you can use DELETE method with the same url as above
