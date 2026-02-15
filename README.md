# Kenwood Productions

A minimal Laravel 11 site showing the Kenwood logo.

## Setup

1. Install dependencies:
   ```bash
   composer install
   ```

2. Generate application key:
   ```bash
   php artisan key:generate
   ```

3. Serve the site (document root must be `public`):
   ```bash
   php artisan serve
   ```
   Then open http://localhost:8000

For production, point your web server (Apache/Nginx) at the `public` directory.

## Structure

- **public/** – Web root; contains `index.php` and `img/kenwood-logo.svg`
- **resources/views/welcome.blade.php** – Home page view (from the original index.html)
- **routes/web.php** – Single route: `GET /` → welcome view

The original `index.html` and `img/` at the project root have been replaced by this Laravel setup; the logo lives at `public/img/kenwood-logo.svg`.
