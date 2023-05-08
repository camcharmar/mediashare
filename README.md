# Media Share (Better Name TBD)

> No more digital rentals!

Browse and borrow from all your friends collective physical media.

## Local Development

The back end is powered by [Laravel](https://laravel.com/), so you will need to be able to run PHP, Composer, and a DB driver such as SQLite, and the front end is [Next.JS](https://nextjs.org/)

### PHP

```bash
$ php -v
PHP 8 or higher
```

Otherwise you can [get PHP here](https://www.php.net/manual/en/install.php)

### Composer

```bash
$ composer --version
Composer version 2.5 or higher
```

Otherwise [get Composer here](https://getcomposer.org/download/)

### SQLite

```bash
$ sqlite3 --version
3.37 or higher
```

Otherwise [here is a SQLite setup guide.](https://dev.to/dendihandian/installing-sqlite3-in-windows-44eb)

Create a file called `database.sqlite` and put it in the `/backend/database` directory.

### Other DB Drivers

If you prefer to use MySQL or PostgreSQL, follow [the Laravel database guides for more details.](https://laravel.com/docs/10.x/database)

### Lets get the backend running!

```bash
$ cd backend
$ cp .env.example .env
$ php artisan migrate
$ php artisan serve
```

Navigating to `localhost:8000` should show

```json
{ "Laravel": "10.9.0" }
```

Leave that running and open another terminal window to configure and serve the front end app.

## Node & NPM

```bash
$ node -v
v18 or higher
```

If you need to install or to upgrade, [heres how to use NVM to manage node](https://nodejs.org/en/download/package-manager#nvm)

```bash
$ npm -v
9.6 or higher
```

If node is up to date you should at least have some version of NPM, to upgrade use `$ npm install -g npm@latest`

## Serving the Frontend

```bash
$ cd frontend
$ cp .env.example .env.local
$ npm install
$ npm run dev
```

Navigate to `http://localhost:3000`. Now you're up and running!
