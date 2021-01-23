# Composer

We need to use the source in China when using Composer in China.

## Mac or Linux

### Make Installation Script

```php
php -r "copy('https://install.phpcomposer.com/installer', 'composer-setup.php');"
```

### Install

```php
php composer-setup.php
```

### Delete Installation Script

```php
php -r "unlink('composer-setup.php');"
```

### Put in the Path

```shell
sudo mv composer.phar /usr/local/bin/composer
```

## Reference

1. [How to Install Composer](https://pkg.phpcomposer.com/#how-to-install-composer)