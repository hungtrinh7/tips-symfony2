# tips-symfony2

A collection of Symfony2 tips.

1. [Dump Symfony data entity](#dump-symfony-data-entity)

### Dump Symfony data entity:

```php
echo '<pre>'; 
\Doctrine\Common\Util\Debug::dump($user); 
echo '</pre>';
```

Very useful when you want to `debug` your code.
