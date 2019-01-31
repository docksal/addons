# PHP Code Sniffer 

Easily run PHPCS and PHPCBF commands to detect violations of a defined coding standard. Coding standards are included within the Docksal `cli` container for both [Drupal](https://www.drupal.org/docs/8/modules/code-review-module/installing-coder-sniffer) and [WordPress](https://github.com/WordPress-Coding-Standards/WordPress-Coding-Standards).

```bash
fin addon install phpcs
```

## Usage once installed

Once installed the following commands can be ran to help with code quality.

### PHPCS

The main `phpcs` script that tokenizes PHP, JavaScript and CSS files to detect violations of a defined coding standard.

```bash
# Default Command
fin phpcs cs "modules/test_module"
```

```bash
# Run With Other Options
fin phpcs cs --standards="ExtraStandards,Drupal,DrupalPractice" modules/test_module
```

### PHPCBF

The second `phpcbf` script automatically corrects coding standard violations. 


```bash
# Default Command
fin phpcs cbf "modules/test_module"
```

```bash
# Run With Other Options
fin phpcs cbf --standards="ExtraStandards,Drupal,DrupalPractice" modules/test_module
```

### Default Standards Used

For Drupal: Drupal,DrupalPractice

For WordPress: WordPress

To customize these the `--standards` option could be used.

Additionally the `PHPCS_STANDARDS` variable may set within `.docksal/docksal.env`.

### Default Extensions Used

For Drupal: php,module,inc,install,test,profile,theme,css,info,txt,md

For WordPress: php

To customize these the `--extensions` option could be used.

Additionally the `PHPCS_EXTENSIONS` variable may set within `.docksal/docksal.env`.
