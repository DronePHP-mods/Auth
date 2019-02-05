# Auth module for DronePHP
### Make it easy

This software is a module for [DronePHP](https://github.com/Pleets/DronePHP).

Visit [DronePHP official](http://www.dronephp.com)

## Installation

Make sure you have a reference to `ifdef` function in your `index.php` and there is a global config file inside `/config`.

```php
require_once("vendor/autoload.php");

function ifdef($value, array $needle)
{
    return \Drone\Util\ArrayDimension::ifdef($needle, include 'config/global.config.php', $value);
}
```

Copy the contents of `src` in the root path of your project and try it!.

To close the current session redirects to `Auth/LogOut/close`.