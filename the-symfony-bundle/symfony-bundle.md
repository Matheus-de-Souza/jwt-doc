# Symfony Bundle

This framework provides a Symfony bundle that will help you to use the components within your Symfony application. The bundle is available

* when you just install the bundle \(`composer require web-token/jwt-bundle`\)
* when you install the whole framework \(`composer require web-token/jwt-framework`\)

If you just install the bundle on an application with Symfony Flex support, then there is nothing to do. Otherwise, you have to register the bundle:

```php
/**
 * {@inheritdoc}
 */
public function registerBundles()
{
    $bundles = [
        ...
        new Jose\Bundle\JoseFramework\JoseFrameworkBundle(),
    ];

    return $bundles;
}
```

The bundle capabilities will depend on the components installed in your application. The core component is always available.

* [Algorithm Management](algorithm-management.md)
* [Header and Claim Checkers](header-and-claim-checker-management.md)
* [Keys and key sets](key-and-key-set-management/)
* [Signed tokens](signed-tokens/)
* [Encrypted tokens](encrypted-tokens/)

