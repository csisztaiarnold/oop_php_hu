# Singleton (egyke)

A singleton csupán egyszer, globálisan példányosított osztály. 

Általában anti-mintának tekintik, mivel merev függőségeket hoz létre az osztályok között és a globális változók működéséhez hasonló azzal a különbséggel, hogy az egykék korlátozhatóak névterületle. Lehetőleg kerüljük a használatát. A singletonokat általában nehéz mockolni. Helyette célszerűbb dependency injectiont használni.

### Mire használható?

- Logoláshoz
- Adatbázis csatlakozáshoz

### Példa

```php
<?php
    class DBConn {

        private static $obj;

        private final function  __construct() {
            echo __CLASS__ . " initializes only once\n";
        }

        public static function getConn() {
            if(!isset(self::$obj)) {
                self::$obj = new DBConn();
            }
            return self::$obj;
        }
    }

    $obj1 = DBConn::getConn();
    $obj2 = DBConn::getConn();

    var_dump($obj1 === $obj2);

```
Eredmény:
```php
DBConn initializes only once
bool(true)
```
