Pagination
=============

[![Total Downloads](https://poser.pugx.org/fafmio/pagination/downloads.svg)](https://packagist.org/packages/fafmio/pagination)
[![Latest Stable Version](https://poser.pugx.org/fafmio/pagination/v/stable.svg)](https://packagist.org/packages/fafmio/pagination)
[![Latest Unstable Version](https://poser.pugx.org/fafmio/pagination/v/unstable.svg)](https://packagist.org/packages/fafmio/pagination)
[![License](https://poser.pugx.org/fafmio/pagination/license.svg)](https://packagist.org/packages/fafmio/pagination)


## Installation

Install with composer:
```shell
composer require "fafmio/pagination:~1.0"
```

## Basic usage

Here's a quick example using the defaults:
```php
use FafMio\Pagination;

$totalItems = 1000;
$itemsPerPage = 50;
$currentPage = 8;
$urlPattern = '/foo/page/(:num)'; // or '/foo?page=(:num)'

$paginator = new Pagination($totalItems, $itemsPerPage, $currentPage, $urlPattern);
```