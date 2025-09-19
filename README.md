<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

You may also try the [Laravel Bootcamp](https://bootcamp.laravel.com), where you will be guided through building a modern Laravel application from scratch.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains thousands of video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the [Laravel Partners program](https://partners.laravel.com).

### Premium Partners

- **[Vehikl](https://vehikl.com)**
- **[Tighten Co.](https://tighten.co)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel)**
- **[DevSquad](https://devsquad.com/hire-laravel-developers)**
- **[Redberry](https://redberry.international/laravel-development)**
- **[Active Logic](https://activelogic.com)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

## Instructions  

### Prerequisites (Initial Requirements for Windows)  

1. **Install PHP**  

- Download PHP from [https://windows.php.net/download/](https://windows.php.net/download/)  
- Choose PHP version **8.1 or newer (Thread Safe)**  
- Extract it into the folder `C:\php`  
- Add `C:\php` to the **PATH environment variable**:  
  - Open **Control Panel → System → Advanced System Settings**  
  - Click **"Environment Variables"**  
  - Under **System Variables**, find **"Path"** and click **Edit**  
  - Add `C:\php`  

- Copy `php.ini-development` and rename it to `php.ini`  
- Edit `php.ini` and uncomment (remove `;`) the following extensions:  
  ```ini
  extension=pdo_pgsql
  extension=pgsql
  extension=openssl
  extension=mbstring
  extension=tokenizer
  extension=curl

2. **Install Composer**

- Download Composer from [https://getcomposer.org/download/]
- Run the Composer-Setup.exe installer
- Follow the installation wizard (make sure the PHP path is correct)
- Restart the command prompt
- Test by running:
- composer --version

3. **Install Node.js and NPM**

- Download Node.js from [https://nodejs.org/]
- Install the latest LTS version
- Restart the command prompt
- Test with:
- node --version
- npm --version

4. **Install PostgreSQL**

- Download PostgreSQL from [https://www.postgresql.org/download/windows/]
- Install PostgreSQL (version 12 or newer)
- During installation:
- Note the password for the postgres user
- Default port: 5432
- Install pgAdmin 4 (GUI tool for managing databases)
- After installation, open pgAdmin 4 to verify the connection

Laravel Installation Steps

1. Install Laravel Installer (Global)

- composer global require laravel/installer
Add Composer global bin ke PATH:
Add C:\Users\username\AppData\Roaming\Composer\vendor\bin ke PATH environment variable

2. Create New Project Laravel

- Open Command Prompt or PowerShell, navigate to the folder where you want to create the project:
  # Method 1: Use Composer (alternative)
  - composer create-project laravel/laravel name-project
  - cd name-project

  # Setup Environment
  - Copy file .env.example become .env
  - Generate application key:
    - php artisan key:generate
  - Edit file .env
   ```ini
   DB_CONNECTION=pgsql
   DB_HOST=127.0.0.1
   DB_PORT=5432
   DB_DATABASE=nama_database
   DB_USERNAME=postgres
   DB_PASSWORD=password_postgresql_anda

