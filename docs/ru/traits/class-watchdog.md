### class-watchdog # ClassWatchdog #> ClassWatchdog {tpl-git PHPDaemon/Traits/ClassWatchdog.php}

```php
namespace PHPDaemon\Traits;
trait ClassWatchdog;
```

> Данная примесь уже использована во всех базовых классах и при наследовании от них не нужно использовать её повторно.

Эта примесь нужна, чтобы предотвратить появление ошибки уровня E_ERROR (Fatal error) при обращении к несуществующему методу. E_ERROR же прерывает работу всего рабочего процесса, что недопустимо в реалиях phpDaemon. Настоятельно рекомендуется к использованию во всех используемых классах.


Определены следующие [магические методы](http://php.net/language.oop5.magic):

-.n.ti `__call` — бросает исключение UndefinedMethodCalled
-.n.ti `__callStatic` — бросает исключение UndefinedMethodCalled
