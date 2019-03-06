# Kint-Smarty

Plugin for [Kint](https://github.com/kint-php/kint) to provide better 
[Smarty](https://smarty.net) support. 

Internal Smarty objects are so big they sometimes hang the browser when dumped. 
This plugin sanitizes the display and only displays minimal, useful data: 
 * Assigned variables (local and global)
 * User-configurable values such as compiled directory and custom functions. 


## Usage

*Zero setup*; install via composer:

```
composer require kint-php/kint-smarty --dev
```

or download [the file](https://raw.githubusercontent.com/kint-php/kint-smarty/master/src/SmartyPlugin.php), include it after 
Kint and register it:

```php
<?php

require 'kint.phar';
require 'SmartyPlugin.php';
Kint::$plugins[] = 'Kint\\Parser\\SmartyPlugin';

```

## Licence

MIT
