## Installing
Follow the steps below to install the bundle.

### Requirements
PHP 5.5.*  
Composer  
Symfony 2.6.*

### Installing
Add `headzoo/polyphonic-symfony` to your composer.json requirements.

```javascript
"require": {
    "headzoo/polyphonic-symfony": "0.0.2"
}
```

Run `composer update` and then add the bundle your AppKernel.php.

```php
class AppKernel extends Kernel
{
    public function registerBundles()
    {
        $bundles = array(
            new Symfony\Bundle\FrameworkBundle\FrameworkBundle(),
            new Symfony\Bundle\SecurityBundle\SecurityBundle(),
            ...
            new Headzoo\Bundle\PolymerBundle\PolymerBundle(),
        )
        
        return $bundles;
    }
}
```