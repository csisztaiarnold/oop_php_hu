#Multiton (többke)

Ugyanaz vonatkozik rá mint a [singleton](singleton.md)-ra, azzal a különbséggel, hogy a multiton többször példányosítható.

###Példa

```php
class Logger
{
    private static $instances = array();

    public static function getInstance($key)
    {
        if(!array_key_exists($key, self::$instances)) {
            self::$instances[$key] = new self();
        }

        return self::$instances[$key];
    }

    // prevent creating multiple instances due to "private" constructor
    private function __construct(){}

    // prevent the instance from being cloned
    private function __clone(){}

    // prevent from being unserialized
    private function __wakeup(){}
}
```

```php
$firstInstance = Logger::getInstance('file');
$secondInstance = Logger::getInstance('email');
```