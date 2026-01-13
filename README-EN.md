<div align="center">

# Dcat Login Captcha

<p>
    <a href="https://github.com/dcat-x/dcat-login-captcha/actions/workflows/tests.yml"><img src="https://github.com/dcat-x/dcat-login-captcha/actions/workflows/tests.yml/badge.svg" alt="Tests"></a>
    <a href="https://packagist.org/packages/dcat-x/dcat-login-captcha"><img src="https://poser.pugx.org/dcat-x/dcat-login-captcha/v/stable" alt="Latest Stable Version"></a>
    <a href="https://packagist.org/packages/dcat-x/dcat-login-captcha"><img src="https://img.shields.io/packagist/dt/dcat-x/dcat-login-captcha.svg" alt="Total Downloads"></a>
    <a href="https://www.php.net/"><img src="https://img.shields.io/badge/php-8.2+-59a9f8.svg" alt="PHP Version"></a>
    <a href="https://github.com/dcat-x/laravel-admin"><img src="https://img.shields.io/badge/dcat--admin-1.0+-59a9f8.svg" alt="Dcat Admin Version"></a>
    <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License"></a>
</p>

**Login captcha extension for [Dcat Admin](https://github.com/dcat-x/laravel-admin)**

English | [简体中文](README.md)

</div>

## Features

- Simple and easy-to-use login captcha
- Customizable captcha length, charset, and dimensions
- Multiple image formats support (PNG, JPEG, GIF)
- Custom font support
- Fully configurable

## Requirements

- PHP >= 8.2
- dcat-x/laravel-admin >= 1.0

## Installation

```bash
composer require dcat-x/dcat-login-captcha
```

After installation, enable this extension in **Admin Panel -> Helpers -> Extensions**.

## Preview

| Example 1 | Example 2 | Example 3 |
|-----------|-----------|-----------|
| ![example1](docs/example1.png) | ![example2](docs/example2.png) | ![example3](docs/example3.png) |

## Configuration

Publish the configuration file (optional):

```bash
php artisan vendor:publish --tag=dcat-login-captcha-config
```

Configuration options:

```php
return [
    // Captcha length
    'length' => 4,

    // Captcha charset
    'charset' => 'abcdefghijklmnpqrstuvwxyz23456789ABCDEFGHIJKLMNOPQRSTUVWXYZ',

    // Captcha image width
    'width' => 150,

    // Captcha image height
    'height' => 43,

    // Image type: png, jpeg, gif
    'type' => 'png',

    // Custom font path (optional)
    'font' => null,

    // Captcha session key
    'captcha_phrase_session_key' => 'login_captcha_phrase',
];
```

## Testing

```bash
composer test
```

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## Contributing

Please see [CONTRIBUTING](.github/CONTRIBUTING.md) for details.

## Security Vulnerabilities

Please review [our security policy](../../security/policy) on how to report security vulnerabilities.

## Credits

- [guanguans](https://github.com/guanguans)
- [cooper](https://github.com/myxiaoao)
- [All Contributors](../../contributors)

## License

The MIT License (MIT). Please see [License File](LICENSE) for more information.
