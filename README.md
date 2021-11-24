# Drupal 8 update tools
Various tools and documentation about Drupal upgrade

## Check plateform requirement
https://www.drupal.org/docs/understanding-drupal/how-drupal-9-was-made-and-what-is-included/environment-requirements-of-drupal-9

## Drupal prior to 8.8
Drupal 8.8 is the first minor release of Drupal 8 that is fully API-compatible with Drupal 9.0.x.
Releases prior to 8.8.0 are unlikely to be compatible with Drupal 9.0.0. We require updating to at least Drupal 8.8.0 prior to updating to Drupal 9 and the upgrade will not proceed until this is done. However more recent patch releases of 8.8.x and 8.9.x will have further bugfixes applied and are always preferred.

## Modules tools
Upgrade Status 
https://www.drupal.org/project/upgrade_status

## Composer commands
```bash
$ composer show drupal/core | grep versions
$ composer require --dev drupal/core-dev:[copy version above] --update-with-all-dependencies
$ composer require drupal/upgrade_status
```

## Upgrade path from 8.7.7 to 8.8
Prevent conflict

```bash
rm -rf vendor
```

### Migrating from webflo/drupal-core-strict to drupal/core-recommended

```bash
composer update # To update any dependencies as a separate step.

```


