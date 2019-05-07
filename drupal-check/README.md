# Drupal-check Docksal Addon

## Installation

```shell
fin addon install drupal-check
```

## Usage

This tool works on all Drupal code.

### 1. Run drupal-check

Usage:

  ```shell
  fin drupal-check [MODULE NAME] [OPTIONS]
  ```

Arguments:

* `MODULE NAME` - The modules machine name.
* `OPTIONS` - See "Options" for allowed values.

Options:

* `-a` Check analysis
* `-d` Check deprecations (default)
* `-t` Module type {core, custom, contrib (default)}

Examples:

* Check the address contrib module:

  ```shell
  fin drupal-check address
  ```

* Check non-contrib module:

  ```shell
  fin drupal-check custom_module -t custom
  ```

* Check the address contrib module for deprecations:

  ```shell
  fin drupal-check address -d
  ```

* Check the address contrib module for analysis:

  ```shell
  fin drupal-check address -a
  ```
