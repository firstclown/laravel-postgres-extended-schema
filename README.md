Laravel Postgres Extended Schema
=========================

[![Latest Version on Packagist][ico-version]][link-packagist]
[![Software License][ico-license]](LICENSE.md)
[![Build Status][ico-travis]][link-travis]
[![Coverage Status][ico-scrutinizer]][link-scrutinizer]
[![Quality Score][ico-code-quality]][link-code-quality]
[![Total Downloads][ico-downloads]][link-downloads]

[ico-version]: https://img.shields.io/packagist/v/phoenixgao/laravel-postgres-extended-schema.svg?style=flat-square
[ico-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
[ico-travis]: https://img.shields.io/travis/phoenixgao/laravel-postgres-extended-schema/master.svg?style=flat-square
[ico-scrutinizer]: https://img.shields.io/scrutinizer/coverage/g/phoenixgao/laravel-postgres-extended-schema.svg?style=flat-square
[ico-code-quality]: https://img.shields.io/scrutinizer/g/phoenixgao/laravel-postgres-extended-schema.svg?style=flat-square
[ico-downloads]: https://img.shields.io/packagist/dt/phoenixgao/laravel-postgres-extended-schema.svg?style=flat-square

[link-packagist]: https://packagist.org/packages/phoenixgao/laravel-postgres-extended-schema
[link-travis]: https://travis-ci.org/phoenixgao/laravel-postgres-extended-schema
[link-scrutinizer]: https://scrutinizer-ci.com/g/phoenixgao/laravel-postgres-extended-schema/code-structure
[link-code-quality]: https://scrutinizer-ci.com/g/phoenixgao/laravel-postgres-extended-schema
[link-downloads]: https://packagist.org/packages/phoenixgao/laravel-postgres-extended-schema

Forked from Bosnadev's original work https://github.com/Bosnadev/Database

## Installation

`$ composer require phoenixgao/laravel-postgres-extended-schema`

## Usage

Add our service provider into `config/app.php`:

```php
<?php
    ...
    'providers' => [
        ...
        Bosnadev\Database\DatabaseServiceProvider::class,
    ],
    ...
```

This library extends PostgreSQL driver for Laravel 5 with support for:

### Additional PostgreSQL data types:
* hstore
* uuid
* geometric types (point, path, circle, line, polygon...)
* network address types

### Table Inheritance
