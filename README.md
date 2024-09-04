# Laravel Nova Grid

## Requirements

- `php: >=8.0`
- `laravel/nova: ^4.0`

## Features

- `->size()` helpers that allow placing items next to one another on the detail and form views

## Installation

Install the package in to a Laravel app that uses [Nova](https://nova.laravel.com) via composer:

```bash
composer require vibar/laravel-nova-grid
```

## Usage

Use `->size()` on any Field.

```php
public function fields(NovaRequest $request)
{
    return [
        Text::make('Email')
          ->size('w-1/12')
          ->sizeHalf(), // w-1/2
          ->sizeOneThird(), // w-1/3
          ->sizeTwoThirds(), // w-2/3
    ];
}
```

## Credits

- [Kaspar Rosin](https://github.com/kasparrosin)

## License

Nova Input Filter is open-sourced software licensed under the [MIT license](LICENSE.md).
