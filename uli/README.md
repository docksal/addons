# Drupal one-time login url

* Generate one time login url and:
  * on Mac copy it to clipboard with `pbcopy`
  * on Linux copy it to both the selection buffer and clipboard with `xclip`

## Usage

```
fin uli [-s] [@drushsitealias] [ drush uli options ]
```

* `-s` outputs the login url with https instead of default of https
* Drush site alias - useful for Drupal multi-site installations
* Drush uli options are passed in. See [Drush user:login documentation](https://drushcommands.com/drush-9x/user/user:login/) for possible options.

Note: the `-s` option and Drush site alias must be one of the first two given on the command line. Both are optional.
