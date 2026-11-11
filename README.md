# Filament_dashboard

A Laravel and Filament administration dashboard for patient, owner, and treatment records.

[Repository](https://github.com/MirzaAlbab/Filament_dashboard)

## Features

- Patient resource with create, edit, and list pages
- Owner and treatment model relationships
- Treatment relation manager
- Patient overview and treatment chart widgets

## Technology

`php` ^8.2 · `filament/filament` ^3.2 · `flowframe/laravel-trend` ^0.3.0 · `laravel/framework` ^11.31 · `laravel/tinker` ^2.9

## Getting started

Install PHP compatible with `composer.json`, Composer, Node.js, and a database supported by the application.

```bash
git clone https://github.com/MirzaAlbab/Filament_dashboard.git
cd Filament_dashboard
```

```bash
composer install
cp .env.example .env
php artisan key:generate
```

Set `APP_URL` and the `DB_*` values in `.env` for your local database. Configure any mail, payment, or other external service used by this project.

```bash
php artisan migrate
npm install
npm run build
php artisan serve
```

Open the URL printed by Artisan. For ongoing frontend development, run `npm run dev` in another terminal.

## Development and checks

```bash
php artisan test
```

Review `tests/` for the current test scope. A configured test runner does not imply coverage of every business workflow.

## Project structure

- `app/` — Application source
- `config/` — Application configuration
- `database/` — Migrations, factories, and seeders
- `public/` — Public web assets and entry points
- `resources/` — Frontend templates and assets
- `routes/` — HTTP route definitions
- `tests/` — Test suite and support files

## Project notes

Uses Laravel 11 and Filament 3. Review app/Providers/Filament/ for panel paths and access configuration. To create a local panel account, use php artisan make:filament-user after database setup.

## Framework

Built with [Laravel](https://laravel.com/docs). Framework packages and third-party dependencies retain their own licenses.

## License

No root `LICENSE` file was present in the reviewed repository. Consult the repository owner about reuse; dependencies and third-party assets retain their own terms.
