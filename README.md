## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling.

## Integrating Laravel 8 with Admin LTE 3 with Auth

**composer global require laravel/installer**

**laravel new adminlte-laravel**
**cd adminlte-laravel**

Need to create database from MySQL same like from .ENV file. Before migrate fixed too length error Inside AppServiceProvider need to add Schema like 

**use Illuminate\Support\Facades\Schema;**

also need to add **Schema::defaultStringLength(191);** in boot function then

**php artisan migrate:fresh**

Now admin lte via composer

**composer require infyomlabs/laravel-ui-adminlte**

To install the AdminLTE theme assets, run the following in the terminal:

**php artisan ui adminlte**

For Integrating Auth Templates

**php artisan ui adminlte --auth**

Last via <a href="https://laravel.com/docs/8.x/mix">Laravel Mix</a> need to run **npm install && npm run dev** or **npm install**
**npm run dev**

if will get compiled successfully screen then run if not then first run **npm run production**

**php artisan serve**
