# Persianalize

**Persianalize** use to normalize Persian input and remove arabic and other similar characters.

## Install

Via Composer

``` bash
$ composer require mahdimajidzadeh/persianalize
```

If you do not run Laravel 5.5 (or higher), then add the service provider in config/app.php:

``` php
MahdiMajidzadeh\Persianalize\PersianalizeServiceProvider:class
```

If you do run the package on Laravel 5.5+, package auto-discovery takes care of the magic of adding the service provider.

## Usage

``` php
$result = Persian::numbers_fa('123٤٥٦'); // return ۱۲۳۴۵۶

$result = Persian::numbers_en('۱۲۳٤٥٦'); // return 123456

$result = Persian::text('ي ڲ ڬ'); // return ی گ ک

$result = Persian::persian($text); // make texts and numbers Persian 

$result = Persian::standard($text); // make texts Persian and numbers English 
```

## Change log

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.
