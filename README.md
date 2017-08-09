# Laravel Personality
The customizable framework for agility for installation and preparation of the environment

## Installed libraries
> [eloquent-sluggable](https://github.com/cviebrock/eloquent-sluggable) @cviebrock

> [flash](https://github.com/laracasts/flash) @laracasts

> [laravel-collective](https://laravelcollective.com/docs/5.4/html) @laravelcollective

> [adminlte-laravel](https://github.com/acacha/adminlte-laravel) @acacha

> [l5-repository](https://github.com/andersao/l5-repository) @andersao

> [laravel-modules](https://github.com/nWidart/laravel-modules) @nWidart

## Providers
```php
    'providers' => [
        // ...
        Cviebrock\EloquentSluggable\ServiceProvider::class,
        Laracasts\Flash\FlashServiceProvider::class,
        Collective\Html\HtmlServiceProvider::class,
        Acacha\AdminLTETemplateLaravel\Providers\AdminLTETemplateServiceProvider::class,
        Prettus\Repository\Providers\RepositoryServiceProvider::class,
        Nwidart\Modules\LaravelModulesServiceProvider::class,
    ];
```
## Aliases
```php
    'aliases' => [
        //...
        'Form' => Collective\Html\FormFacade::class,
        'Html' => Collective\Html\HtmlFacade::class,
        'AdminLTE' => Acacha\AdminLTETemplateLaravel\Facades\AdminLTE::class,
        'Module' => Nwidart\Modules\Facades\Module::class,
    ],
```
## Publish
```shell
    php artisan vendor:publish --provider="Cviebrock\EloquentSluggable\ServiceProvider"
    php artisan vendor:publish --provider="Laracasts\Flash\FlashServiceProvider"
    php artisan vendor:publish --tag=adminlte --force
    php artisan vendor:publish --provider "Prettus\Repository\Providers\RepositoryServiceProvider"
    php artisan vendor:publish --provider="Nwidart\Modules\LaravelModulesServiceProvider"
``` 
    
## Copyright and License

Was written by [brunosite](http://brunosite.com) and is released under the 
[MIT License](LICENSE.md).

Copyright (c) 2017 Bruno Site