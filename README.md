# Pizza House (Laravel)

> A pizza-ordering web app built with Laravel 7: customers place orders, and logged-in staff can view, review and complete them.

![PHP](https://img.shields.io/badge/PHP-777BB4?logo=php&logoColor=white)
![Laravel](https://img.shields.io/badge/Laravel-FF2D20?logo=laravel&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?logo=bootstrap&logoColor=white)

## Features

- **Order form:** pick the pizza type, base and toppings (`/pizzas/create`).
- **Authentication:** registration and login with Laravel's built-in auth scaffolding.
- **Orders dashboard (staff only):** list all orders, view an order, and mark it as complete (delete).
- **MVC structure:** resource-style routes, `PizzaController`, Eloquent models, migrations and Blade templates.

## Routes

| Method | URL | Action | Auth |
| --- | --- | --- | --- |
| GET | `/pizzas` | List orders | ✔ |
| GET | `/pizzas/create` | Order form | |
| POST | `/pizzas` | Save an order | |
| GET | `/pizzas/{id}` | Order details | ✔ |
| DELETE | `/pizzas/{id}` | Complete (delete) an order | ✔ |

## Run it

```bash
git clone https://github.com/AhmedGamal98/laravel-pizza-house.git
cd laravel-pizza-house
composer install
cp .env.example .env          # then set DB_DATABASE, DB_USERNAME, DB_PASSWORD
php artisan key:generate
php artisan migrate
php artisan serve
```

Requires PHP 7.2.5+, Composer and MySQL.

## Author

**Ahmed Gamal Saber**, Full-Stack Web Developer & AI Engineer
[LinkedIn](https://linkedin.com/in/ahmed-gamal-saber-382081169) · [GitHub](https://github.com/AhmedGamal98)
