<img src="https://i.ibb.co/gzcpNv5/Banner-Package.png" alt="preview of package" width="100%"/>

<p align="center">
    <a href="https://packagist.org/packages/koalafacade/filament-alertbox"><img src="https://img.shields.io/packagist/v/KoalaFacade/filament-alertbox?color=F28D1A&style=for-the-badge" alt="Packagist"/></a>
    <a href="https://github.com/KoalaFacade/Filament-Alertbox/actions/workflows/run-tests.yml"><img src="https://img.shields.io/github/actions/workflow/status/KoalaFacade/Filament-Alertbox/run-tests.yml?branch=main&label=test&style=for-the-badge" alt="Test Passing"/></a>
    <a href="https://laravel.com"><img src="https://img.shields.io/badge/Laravel-^9.x-red?style=for-the-badge&logo=Laravel" alt="Laravel" /></a>
    <a href="https://php.net"><img src="https://img.shields.io/badge/PHP-8.1-7A86B8?style=for-the-badge&logo=php" alt="PHP Badge"/></a>
</p>



> Filament plugin to handle an alert box in your form page

## Installation
You can install the package via composer: 
```bash
composer require koalafacade/filament-alertbox
```

## Usage

```php
use KoalaFacade\FilamentAlertBox\Forms\Components\AlertBox

AlertBox::make()
    ->label(label: 'Oops')
    ->helperText(label: 'please make a payment first.')
    ->icon(name: 'heroicon-o-exclamation')
    ->warning();
```

## Available Method
This field has most of the same functionality of the Field class
 ```php
  /** define alert type */
  function primary(): static;
  function warning(): static;
  function success(): static;
  function danger(): static;

  /** hide alert box */
  function hidden(bool | Closure $condition = true): static;
  function hiddenOn(string | array $contexts): static;

  /** define alert icon */
  function hiddenOn(string | array $contexts): static;
 ```

## License
The MIT License (MIT). Please see [License File](https://github.com/KoalaFacade/Filament-Alertbox/blob/main/LICENSE.md) for more information.

