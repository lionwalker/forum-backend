## Installation

Clone the repo locally:

```sh
git clone https://github.com/lionwalker/forum-backend.git forum-backend
cd forum-backend
```

Install PHP dependencies:

```sh
composer install
```

Install NPM dependencies:

```sh
npm install
```

Build assets:

```sh
npm run dev
```

Setup configuration:

```sh
cp .env.example .env
```

Generate application key:

```sh
php artisan key:generate
```

Create an SQLite database. You can also use another database (MySQL, Postgres), simply update your configuration accordingly.

```sh
touch database/database.sqlite
```

Run database migrations:

```sh
php artisan migrate
```

Run database seeder:

```sh
php artisan db:seed
```

Run the dev server (the output will give the address):

```sh
php artisan serve
```

You're ready to go! Visit forum in your browser, and login with:

- **Username:** admin@admin.com
- **Password:** Admin@123

### API documentation

- https://documenter.getpostman.com/view/11193587/TzmCgD5L

### Proposed improvements

- Can implement authorization part by using packages like spatie permissions
- Can implement activity log easily with packages like spatie activity logs

### Notes

- Added CROS middleware to enable Access-Control-Allow-Methods 
