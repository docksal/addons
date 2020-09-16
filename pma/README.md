# PHPMyAdmin - Docksal addon

Easily install PHPMyAdmin for your Docksal project. Make it easy to access the database and examine directly rather then through the CLI.

```bash
fin addon install pma
```

## URL

After the installation PhpMyAdmin will be available at `http://pma-<project_name>.docksal`

## Command line reference

- `fin pma disable` to disable
- `fin pma enable` to re-enable

## Regressions
 Previously the url for PHPMyAdmin could be found at `http://pma.<project_name>.docksal`. This change was made to make it easier to use a LetsEncrypt wildcard certificate, as it is only valid for one level of subdomains.
