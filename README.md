# Office Management System (Laravel)

A simple Office Management System built using **Laravel**, **MySQL**, **Blade**, **TailwindCSS (CDN)**, and **jQuery DataTables**. This project includes basic CRUD for companies and employees with a clean UI and searchable employee table.

## Features
- Add, view, and delete companies
- Add, view, and delete employees
- Assign each employee to a company
- Employee list with search, sort, and pagination (DataTables)
- Simple styling using Tailwind via CDN (no npm build needed)

## Setup

### Install Dependencies
composer install

### Environment Setup
cp .env.example .env

Update `.env`:
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_db_name
DB_USERNAME=your_db_user
DB_PASSWORD=your_db_pass

### Generate Key
php artisan key:generate

### Run Migrations
php artisan migrate

### Start Server
php artisan serve

Open in browser:
http://127.0.0.1:8000

## Routes

### Companies
- GET /companies
- GET /companies/create
- POST /companies
- DELETE /companies/{id}

### Employees
- GET /employees
- GET /employees/create
- POST /employees
- DELETE /employees/{id}

## Notes
This project is made for practice and assignments to understand Laravel CRUD, migrations, Blade views, Tailwind styling, and DataTables search/pagination.