# PhpSpec extension for PHPStan

[![Minimum PHP Version](https://img.shields.io/badge/php-%3E%3D%207.1-8892BF.svg)](https://php.net/)
[![Latest Stable Version](https://img.shields.io/packagist/v/proget-hq/phpstan-phpspec.svg)](https://packagist.org/packages/proget-hq/phpstan-phpspec)
[![Build Status](https://travis-ci.org/proget-hq/phpstan-phpspec.svg?branch=master)](https://travis-ci.org/proget-hq/phpstan-phpspec)
[![Total Downloads](https://poser.pugx.org/proget-hq/phpstan-phpspec/downloads.svg)](https://packagist.org/packages/proget-hq/phpstan-phpspec)
[![License](https://poser.pugx.org/proget-hq/phpstan-phpspec/license.svg)](https://packagist.org/packages/proget-hq/phpstan-phpspec)

## What does it do?

* Provides correct return type for `Collaborator` in spec methods
  * `will*` methods
* Provides correct methods for `ObjectBehavior`:
  * `should*` methods
  * `beConstructedWith`, `beConstructedThrough`, `beAnInstanceOf`

## Compatibility

| PHPStan version | PhpSpec extension version |
| --------------- | ---------------------- |
| 0.10.7          | 0.1.x                  |


## Installation

```sh
composer require --dev proget-hq/phpstan-phpspec
```

## Configuration

Put this into your `phpstan.neon` config:

```neon
includes:
	- vendor/proget-hq/phpstan-phpspec/extension.neon
parameters:
    phpspecSourceFiles:
        - 'src/'
```

## Limitations

TBD.
