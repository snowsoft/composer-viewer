# Composer Viewer for Laravel-admin

A web interface of composer packages in laravel.

## Screenshot

![screenshot](https://user-images.githubusercontent.com/2421068/46718077-a7fadc00-cc9c-11e8-9219-c8a2bac1219e.png)

## Installation

> Before you install, make sure PHP exec() function is enabled in your php.ini config file.

```bash
composer require snowsoft/composer-viewer
# If you want to add a link entry in the left menu, use the following command to import
php artisan admin:import composer-viewer
```

## Configuration

In the extensions section of the config/admin.php file, add configurations

```php
'extensions' => [
    'composer-viewer' => [
        // Set this to false if you want to disable this extension
        'enable' => true,
        // Set the location of composer command
        'which-composer' => '/usr/local/bin/composer', // !! it's important !!
    ]
]
```

## Usage
Open http://your-host/admin/composer-viewer

And you can find these installed packages.

## More resources

[Awesome Laravel-admin](https://github.com/jxlwqq/awesome-laravel-admin)

## License

Licensed under [The MIT License (MIT)](LICENSE).
