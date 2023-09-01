### Install jestream and livewire

composer require laravel/jetstream
php artisan jetstream:install livewire
npm install
npm run dev
php artisan migrate

### Install And configure elements

-   Excel -> composer require maatwebsite/excel -W

#### Add Service providers in config/app.php

'providers' => [Maatwebsite\Excel\ExcelServiceProvider::class]
'aliases' => ['Excel' => Maatwebsite\Excel\Facades\Excel::class]

## Publish excel configuration

php artisan vendor:publish --provider="Maatwebsite\Excel\ExcelServiceProvider" --tag=config

## Migrations, Controllers, Seeders, Factories, Resource
