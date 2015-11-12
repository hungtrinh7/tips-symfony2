# tips-symfony2

A collection of Symfony2 tips.

1. [Dump entity data](#dump-entity-data)
2. [Flash message](#flash-message)

### Dump entity data:

```php
echo '<pre>'; 
\Doctrine\Common\Util\Debug::dump($user); 
echo '</pre>';
```

Very useful when you want to `debug` your code.

### Flash message:

```php
// in Controller
$this->addFlash(
    'notice',
    'message content'
);
```

``` twig
{# in Twig #}
{% for flashMessage in app.session.flashbag.get('notice') %}
    <div class="flash-notice">
        {{ flashMessage }}
    </div>
{% endfor %}
```
