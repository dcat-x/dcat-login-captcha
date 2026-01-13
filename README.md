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

**[Dcat Admin](https://github.com/dcat-x/laravel-admin) 登录验证码扩展**

[English](README-EN.md) | 简体中文

</div>

## 功能特性

- 简单易用的登录验证码
- 支持自定义验证码长度、字符集、尺寸
- 支持多种图片格式 (PNG、JPEG、GIF)
- 支持自定义字体
- 完全可配置

## 环境要求

- PHP >= 8.2
- dcat-x/laravel-admin >= 1.0

## 安装

```bash
composer require dcat-x/dcat-login-captcha
```

安装完成后，在后台 **开发工具 -> 扩展** 中启用本扩展。

## 预览

| 示例 1 | 示例 2 | 示例 3 |
|--------|--------|--------|
| ![example1](docs/example1.png) | ![example2](docs/example2.png) | ![example3](docs/example3.png) |

## 配置

发布配置文件（可选）:

```bash
php artisan vendor:publish --tag=dcat-login-captcha-config
```

配置项说明:

```php
return [
    // 验证码长度
    'length' => 4,

    // 验证码字符集
    'charset' => 'abcdefghijklmnpqrstuvwxyz23456789ABCDEFGHIJKLMNOPQRSTUVWXYZ',

    // 验证码图片宽度
    'width' => 150,

    // 验证码图片高度
    'height' => 43,

    // 图片类型: png, jpeg, gif
    'type' => 'png',

    // 自定义字体路径 (可选)
    'font' => null,

    // 验证码 Session 键名
    'captcha_phrase_session_key' => 'login_captcha_phrase',
];
```

## 测试

```bash
composer test
```

## 变更日志

请参阅 [CHANGELOG](CHANGELOG.md) 获取最近有关更改的更多信息。

## 贡献指南

请参阅 [CONTRIBUTING](.github/CONTRIBUTING.md) 有关详细信息。

## 安全漏洞

请查看[安全政策](../../security/policy)了解如何报告安全漏洞。

## 贡献者

- [guanguans](https://github.com/guanguans)
- [cooper](https://github.com/myxiaoao)
- [所有贡献者](../../contributors)

## 协议

MIT 许可证 (MIT)。有关更多信息，请参见[协议文件](LICENSE)。
