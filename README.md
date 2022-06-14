# Omnipay: Example Application

This is an example web application built using the [Silex micro-framework](http://silex.sensiolabs.org/).
It demonstrates using Omnipay to process payments using all supported payment gateways.

## Getting Started

To run the example application, you must first install the development dependencies via composer.
From the root `omnipay` directory, run `composer install`.

## Starting PHP local server
php -S localhost:8000

## Configuration

Only mpesa gateway is installed by default. You can require the gateways you want to test with Composer, eg:

```
composer require omnipay/omnipay-mpesa
```

Then add the gateway to the `gateways.php` configuration file.

To test Mpesa gateway, you will need to have access to valid credentials. To obtain valid credentials,
contact the payment gateway's support.

You can configure a gateways settings in the application. All data is stored using regular PHP
sessions, so will not be persisted between sessions.

## Support

If you are having general issues with Omnipay, we suggest posting on
[Stack Overflow](http://stackoverflow.com/). Be sure to add the
[omnipay tag](http://stackoverflow.com/questions/tagged/omnipay) so it can be easily found.

If you want to keep up to date with release anouncements, discuss ideas for the project,
or ask more detailed questions, there is also a [mailing list](https://groups.google.com/forum/#!forum/omnipay) which
you can subscribe to.

If you believe you have found a bug, please report it using the [GitHub issue tracker](https://github.com/thephpleague/omnipay-example/issues),
or better yet, fork the library and submit a pull request.
