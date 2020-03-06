# Drupal one-time login url

* Generate one time login url and:
  * on Mac copy it to clipboard with `pbcopy`
  * on Linux copy it to both the selection buffer and clipboard with `xclip`

## Usage

```
fin uli [-s] [-i] [@drushsitealias] [ drush uli options ]
```

* `-s` outputs the login url with https instead of default of https
* Setting `DOCKSAL_ADDON_ULI_USE_HTTPS=1` in the global `docksal.env` or in a project's `docksal-local.env` will force the use of https in the link output unless overridden by the `-i` option.
* `-i` outputs the login url with the default http
* Drush site alias - useful for Drupal multi-site installations
* Drush uli options are passed in. See [Drush user:login documentation](https://drushcommands.com/drush-9x/user/user:login/) for possible options.

Note: the `-s` and `-i` options and Drush site alias must be one of the first two given on the command line. Both are optional.
