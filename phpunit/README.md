# PHPUnit

Easily run PHPUnit tests for your Drupal 8 project.

```bash
fin addon install phpunit
```

## Usage once installed

Run `fin phpunit` to run the tests. Any additional arguments and options will be appended to the command. For example, to run tests within the `modules/custom` directory, run `fin phpunit modules/custom`.

If no `phpunit.xml` file exists, either a project specific one can be copied from `.docksal/drupal/core/phpunit.xml` or core's `phpunit.xml.dist` will be duplicated and renamed.
