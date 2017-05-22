[![Version 2.3.0](https://img.shields.io/badge/version-v0.0.1-green.svg)](:release:)
[![Build Status](https://travis-ci.org/jorge-matricali/jtrace.svg?branch=master)](:status:) [![Coverage Status](https://coveralls.io/repos/github/jorge-matricali/jtrace/badge.svg?branch=master)](https://coveralls.io/github/jorge-matricali/jtrace?branch=master) 
[![MIT licensed](https://img.shields.io/github/license/jorge-matricali/jtrace.svg)](https://raw.githubusercontent.com/jorge-matricali/jtrace/master/LICENSE.txt) [![Packagist](https://img.shields.io/packagist/dt/jorge-matricali/jtrace.svg)](https://packagist.org/packages/jorge-matricali/jtrace)

# jTrace PHP
Prints PHP exceptions in a Java style :)

## Installation

You can add this library as a dependency to your project using [Composer](https://getcomposer.org/):

    composer require jorge-matricali/jtrace

If you only need this library during development, then you should install using:

    composer require --dev jorge-matricali/jtrace

### Usage

```php
use JorgeMatricali\JTrace;

try {
    // ...
} catch (Exception $e) {
    echo JTrace::print($e);
}
```

The code above yields the output below:

Phalcon\Mvc\Dispatcher\Exception: IndexController handler class cannot be loaded at Phalcon.Mvc.Dispatcher._throwDispatchException(index.php:93) at Phalcon.Dispatcher._dispatch(Unknown Source) at Phalcon.Dispatcher.dispatch(Unknown Source) at Phalcon.Mvc.Application.handle(Unknown Source) ... 1 more
