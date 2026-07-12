# Laravel Roles & Permissions Starter

A Laravel starter project set up for role- and permission-based access control, built as a base for adding RBAC to a Laravel application.

## What's inside

- `spatie/laravel-permission` installed with its roles/permissions database tables migrated
- `laravel/sanctum` for API token authentication
- `laravel/jetstream` included as a dependency for future auth scaffolding
- Standard Laravel application skeleton (default routes, models, and migrations)

Note: role/permission assignment is not yet wired into the `User` model or routes — this repo currently provides the installed packages and migrated schema as a foundation.

## Tech stack

- PHP / Laravel
- MySQL
- Sanctum, Jetstream, spatie/laravel-permission

## Quickstart

```bash
composer install
cp .env.example .env
php artisan key:generate

# configure DB_* in .env, then:
php artisan migrate

npm install
npm run dev

php artisan serve
```

App: http://localhost:8000

## Structure

```
app/                Application code (models, providers, HTTP)
routes/             Web and API routes
database/migrations Schema, including the permission tables
config/permission.php  spatie/laravel-permission configuration
```
