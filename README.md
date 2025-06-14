
# Public Blog API

Public blog API. For OpenAPI documentations visit `app.url/docs/api`




## Features
- JWT authentication
- Post categories
- Comments & replies
- Likes & dislikes using Redis
- Admin endpoints



## Installation
Alternative installation is possible without local dependencies relying on [Docker](#Docker).

Clone the repository
```bash
  git clone https://github.com/alimaatin/laravel-blog-api
  cd laravel-blog-api
```
Install all the dependencies
```bash
composer install
npm install
```
Copy the example env file and make the required configuration changes in the .env file
```bash
cp .env.example .env
```
Generate a new application key
```bash
php artisan key:generate
```
Generate a new JWT secret
```bash
php artisan key:generate
```
Create storage link for file uploads
```bash
php artisan storage:link
```
Run the database migrations
```bash
php artisan migrate
```
Start the local development server
```bash
composer run dev
```
Seed the database(optional)
```bash
php artisan db:seed
```
## Docker
This Laravel project uses Laravel Sail, a lightweight command-line interface for interacting with Docker. Sail provides a simple starting point for building a Laravel application using PHP, MySQL, and other common services within Docker containers.

To get the project running simply use
```bash
./vendor/bin/sail up
```
Or in the background
```bash
./vendor/bin/sail up -d
```

Once the application's containers have been started, you may access the project in your web browser at: http://localhost.
