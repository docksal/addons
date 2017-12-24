# Redis

Easily install Redis to the project

```bash
fin addon install redis
```

## Usage once installed

- `fin redis disable` to disable
- `fin redis enable` to re-enable

## More documentation

- Download redis from https://www.drupal.org/project/redis
- No need to enable the module
- Edit /sites/default/settings.local.php and add the following lines.
	- $conf['redis_client_interface'] = 'PhpRedis'; // Can be "Predis".
  - $conf['redis_client_host']      = 'redis';  // Your Redis instance hostname.
  - $conf['lock_inc']               = 'sites/all/modules/contrib/redis/redis.lock.inc';
  - $conf['path_inc']               = 'sites/all/modules/contrib/redis/redis.path.inc';
  - $conf['cache_backends'][]       = 'sites/all/modules/contrib/redis/redis.autoload.inc';
  - $conf['cache_default_class']    = 'Redis_Cache';
