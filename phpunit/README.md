# PHPUnit

Easily run PHPUnit tests for your Drupal 8 project.

```bash
fin addon install phpunit
```

## Usage once installed

Run `fin phpunit` to run tests. Any additional options such as the directory to look for tests with be appended to the command.

If no `phpunit.xml` file exists, one will be copied from either `.docksal/drupal/core/phpunit.xml` or `core/phpunit.xml.dist`.
