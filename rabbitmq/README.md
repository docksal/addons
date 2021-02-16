# RabbitMQ

Easily install RabbitMQ service to the project

```bash
fin addon install rabbitmq
```

## Usage once installed

- `fin rabbitmq disable` to disable
- `fin rabbitmq enable` to re-enable

## Host and Port

From within your project, the rabbitmq service will be available at `rabbitmq:5672`

## URL

After the installation RabbitMQ Management UI will be available at `http://rabbitmq-<project_name>.docksal` with the default username and password of `guest / guest`.
