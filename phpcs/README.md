# PHP Codesniffer

Easily run PHPCS and PHPCBF commands to help with coding standards. Coding standards are included within the
Docksal `cli` container for both [Drupal](https://www.drupal.org/docs/8/modules/code-review-module/installing-coder-sniffer) and [WordPress](https://github.com/WordPress-Coding-Standards/WordPress-Coding-Standards).

```bash
fin addon install phpcs
```

## Usage once installed

Once installed the following commands can be ran to

### PHPCS

PHP CodeSniffer detects violations of a defined coding standard.

```bash
# Default Command
fin phpcs cs "modules/test_module"
```

```bash
# Run With Other Options
fin phpcs cs --standard="ExtraStandards,Drupal,DrupalPractice" modules/test_module
```

### PHPCBF

PHP Code Beautifier and Fixer fixes violations of a defined coding standard.


```bash
# Default Command
fin phpcs cbf "modules/test_module"
```

```bash
# Run With Other Options
fin phpcs cbf --standard="ExtraStandards,Drupal,DrupalPractice" modules/test_module
```

### Default Standards Used

For Drupal: Drupal,DrupalPractice
For WordPres: WordPress

To customize these the `--standard` option could be used.
Additionally the `PHPCS_STANDARD` variable may set within `.docksal/docksal.env`.

### Default Extensions Used

For Drupal: php,module,inc,install,test,profile,theme,css,info,txt,md
For WordPress: php

To customize these the `--extension` option could be used.
Additionally the `PHPCS_EXTENSION` variable may set within `.docksal/docksal.env`.
