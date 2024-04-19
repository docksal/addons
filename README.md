# Docksal addons

Required fin version is 1.7.0 or higher.

Addons is a **community driven** project. If you have an addon idea, we will gladly welcome the new addon.

DISCLAMER: since it is a community driven project it is only smoke-tested and code is only reviewed for vulnerabilities. Addons may not always be up to date with the latest Docksal practices or might have bugs. Feel free to raise issues or pull requests to fix those bugs.

# Addons list

| Name	                     |  Description  |  Requirements 	 |
|----------------------------|---------------|-----------------|
| **[example](example)**	   |  A working documentation on what is Docksal addon and how it works 	|  |
| [adminer](adminer)         | [Adminer](https://www.adminer.org/) database management tool | MySQL |
| [andock](andock)           | [Andock](https://andock.readthedocs.io/en/latest/) makes it dead simple to get Docksal environments up on your server. | Docksal |
| [artisan](artisan)         | Runs [Laravel's Artisan](https://laravel.com/docs/artisan) command in `cli`. **Requires** artisan pre-installed inside `cli`. | Laravel, Artisan |
| [blt](blt)                 | Acquia BLT tool launcher (requires [BLT installation](https://blog.docksal.io/docksal-and-acquia-blt-1552540a3b9f)) | Drupal |
| [codeclimate](codeclimate) | [CodeClimate](https://codeclimate.com/) code quality tool | |
| [dbeaver](dbeaver)         | Launches [DBeaver](https://dbeaver.io/) with the connection information for current project. | macOS, Linux |
| [mailpit](mailpit)         | [Mailpit](https://github.com/axllent/mailpit) email capture service for current project |  |
| [meilisearch](meilisearch) | [Meilisearch](https://www.meilisearch.com/) search for local development | |
| [mkcert](mkcert)           | [mkcert](https://github.com/FiloSottile/mkcert) addon for Docksal |  |
| [phpcs](phpcs)             | PHP Code Sniffer and Code Beautifier | |
| [phpunit](phpunit)         | Creates a phpunit.xml file and runs PHPUnit tests | Drupal |
| [pma](pma)                 | [PhpMyAdmin](https://www.phpmyadmin.net/) database management tool | MySQL |
| [pull](pull)               | Pull assets from hosting environment to local | Drupal |
| [rabbitmq](rabbitmq)       | [RabbitMQ](https://www.rabbitmq.com/) Message Broker | RabbitMQ |
| [redis](redis)             | Add [Redis](https://redis.io/) to current project |  |
| [sequelace](sequelace)     | Launches [SequelAce](https://github.com/Sequel-Ace/Sequel-Ace) with the connection information for current project. | macOS |
| [sequelpro](sequelpro)     | Launches [SequelPro](https://www.sequelpro.com) with the connection information for current project. | macOS |
| [simpletest](simpletest)   | Runs SimpleTest tests in Drupal 7 and 8 | Drupal |
| [sitediff](sitediff)       | Runs Sitediff tests in your Docksal project | |
| [soketi](soketi)           | [Socketi](https://docs.soketi.app/) Soketi is your simple, fast, and resilient open-source WebSockets server |  |
| [solr](solr)               | [Apache Solr](http://lucene.apache.org/solr/) search service for current project |  |
| [tableplus](tableplus)     | Launches [TablePlus](https://www.tableplus.com) with the connection information for current project. | macOS |
| [uli](uli)                 | Generate one time login url for current site | Drupal |
| [wkhtmltopdf](wkhtmltopdf) | Installs wkhtmltopdf 0.12.5 with QT compiled in. |  |
| [xdebug](xdebug)           | Turns [xdebug](https://docs.docksal.io/tools/xdebug/) on or off and restarts docksal |  |
