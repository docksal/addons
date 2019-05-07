# Drupal-check Docksal Addon

## Installation

Download or clone the drupal-check addon and place it into your .docksal/addons directory.

```shell
cd .docksal/addons
git clone https://github.com/cbarrettgenuine/drupal-check.git
fin addon install drupal-check
```

__Note: If you want this to remain part of your project's repo, delete the `.git` folder from within the `.docksal/addons/drupal-check` folder__

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
* `-t` Module type {core, custom, profile, contrib (default)}
* `-p` Profile name for multi-sites if using a profile type module
* `-v` Verbose output

Assumptions:

The `-p profile_name` and `-t profile` arguments assume that your profile and modules follow this directory structure:
```
/var/www/DOCROOT/profiles/custom/PROFILE_DIR/modules/MODULE_NAME
```
The command `fin drupal-check my_profile_module -a -t profile -p my_profile_name` will look for your module in:
```
/var/www/DOCROOT/profiles/custom/my_profile_name/modules/my_profile_module
```

In the event that this does not match your path, you can use a local.drupal-check file. For best results, copy and rename the `example.local.drupal-check` file and add your path to the `CUSTOM` variable.

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

* Check a custom, profile specific module for analysis:

  ```shell
  fin drupal-check my_profile_module -a -t profile -p my_profile_name
  ```

* Check a custom module for analysis with verbose output:

  ```shell
  fin drupal-check my_custom_module -a -t custom -v
  ```
