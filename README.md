<p align="center">
    <img src="https://github.com/wintercms/winter/raw/develop/modules/backend/assets/images/wordmark.png?raw=true" alt="Winter CMS Logo" width="100%" />
</p>

- [Website Winter CMS](https://wintercms.com)
- [Docs](https://wintercms.com/docs/)
- [GitHub](https://github.com/wintercms/winter/)

## Install

### WinterCMS

Installing Winter via Composer is easy. You can use the `create-project` command through Composer to quickly set up a new Winter installation.

```bash
composer create-project wintercms/winter <your installation directory>

# Example:
#   composer create-project wintercms/winter mywinter
```

If you wish to install a specific version of Winter, you can also specify the version.

```bash
composer create-project wintercms/winter <your installation directory> "<version>"

# Example:
#   composer create-project wintercms/winter mywinter "1.0.474"
```

Read more in the [documentation](https://wintercms.com/docs/help/using-composer).

### Example of a minimal project

```bash
# Install Winter CMS, plugin with tools and default theme
composer create-project wintercms/winter mysite
composer require for-wintercms/wn-toolbox-plugin
composer require for-wintercms/wn-default-theme

# Generate a configuration file (.env)
php artisan winter:env

# DB migration
php artisan winter:up

# Generates a mirrored public folder using symbolic links.
php artisan winter:mirror public/
```
