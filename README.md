# Laravel 13 with Inertia JS and Vue 3

This is a Laravel 13 project configured with Inertia JS and Vue 3 for modern full-stack development.

## Getting Started

### Prerequisites
- PHP 8.2 or higher
- Composer
- Node.js 18+ and npm/yarn

### Installation

1. **Install PHP dependencies:**
   ```bash
   composer install
   ```

2. **Install JavaScript dependencies:**
   ```bash
   npm install
   ```

3. **Set up environment:**
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

4. **Run migrations (if any):**
   ```bash
   php artisan migrate
   ```

### Development

1. **Start the development server:**
   ```bash
   php artisan serve
   ```

2. **In another terminal, start Vite for frontend development:**
   ```bash
   npm run dev
   ```

The application will be available at `http://localhost:8000`.

### Production Build

Build assets for production:
```bash
npm run build
```

## Project Structure

```
├── app/                 # Laravel application code
├── resources/
│   └── js/
│       ├── app.js      # Inertia app entry point
│       ├── bootstrap.js # Axios configuration
│       ├── Layouts/    # Vue layout components
│       └── Pages/      # Vue page components
├── routes/             # Laravel routes
├── vite.config.js      # Vite configuration
├── package.json        # Node dependencies
└── composer.json       # PHP dependencies
```

## Creating Pages

1. Create a Vue component in `resources/js/Pages/`
2. Return it from a Laravel route controller using Inertia:
   ```php
   return Inertia::render('YourPage', [
       'prop' => 'value'
   ]);
   ```

## Documentation

- [Laravel 13 Documentation](https://laravel.com/docs/13)
- [Inertia JS Documentation](https://inertiajs.com)
- [Vue 3 Documentation](https://vuejs.org)