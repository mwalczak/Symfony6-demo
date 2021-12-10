Symfony Demo Application
========================

The "Symfony Demo Application" is a reference application created to show how
to develop applications following the [Symfony Best Practices][1].

Requirements
------------

  * docker
  * docker-compose
  
Usage
-----

Start docker with this command:

```bash
$ docker-compose up -d
$ docker-compose exec php composer install
$ docker-compose exec php chmod -R o+w var/log
```

Then access the application in your browser at the given URL (<https://localhost:8085> by default).

Tests
-----

Execute this command to run tests:

```bash
$ docker-compose exec php bin/phpunit
```

[1]: https://symfony.com/doc/current/best_practices.html
[2]: https://symfony.com/doc/current/reference/requirements.html
[3]: https://symfony.com/doc/current/cookbook/configuration/web_server_configuration.html
[4]: https://symfony.com/download
