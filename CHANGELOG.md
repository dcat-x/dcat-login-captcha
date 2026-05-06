# Changelog

All notable changes to `dcat-x/dcat-login-captcha` will be documented in this file.

## [Unreleased]

## [1.2.0] - 2026-05-06

### Changed

- Support `dcat-x/laravel-admin` `^1.0 || ^2.0` (Laravel 12 & 13)
- Loosen `orchestra/testbench` to `^10.0 || ^11.0`
- Loosen `phpunit/phpunit` to `^11.0 || ^12.0`

## [1.1.1] - 2025-01-13

### Fixed

- Fix duplicate captcha display in multi-application environments (e.g., admin + admin-merchant)

## [1.1.0] - 2025-01-13

### Changed

- Fork from `guanguans/dcat-login-captcha`
- Update package name to `dcat-x/dcat-login-captcha`
- Require PHP 8.2+
- Require `dcat-x/laravel-admin` ^1.0 (Laravel 12 support)
- Update PHPUnit to v11
- Replace Psalm with PHPStan/Larastan for static analysis
- Update all GitHub Actions to latest versions
- Modernize code style with PHP CS Fixer
