# NestJS MongoDB RabbitMQ Docker

A microservices application using RabbitMQ as our message broker
Application based on NestJS, where MongoDB a database.
All this is packed in Docker-Compose, in Docker we use bitnami/mongodb.

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="17%">
      <a href="https://nestjs.com/">
        <img height="50" alt="NestJS" src="https://hsto.org/getpro/habr/post_images/d11/98b/ac8/d1198bac8e4ced0d89d5e5983061f418.png"/>
      </a>
      <br />
      NestJS
    </td>
    <td align="center" valign="middle" width="17%">
      <a href="https://www.mongodb.com/">
      <img height="50" alt="PostgresSQL" src="https://w7.pngwing.com/pngs/429/921/png-transparent-mongodb-plain-wordmark-logo-icon-thumbnail.png"/>
      </a>
      <br />
      MongoDB
    </td>
    <td align="center" valign="middle" width="17%">
      <a href="https://www.rabbitmq.com/">
      <img height="50" alt="TypeORM" src="https://seeklogo.com/images/R/rabbitmq-logo-25641A76DE-seeklogo.com.png"/>
      </a>
      <br />
      RabbitMQ
    </td>
    <td align="center" valign="middle" width="17%">
      <a href="https://www.docker.com/">
      <img height="50" alt="Docker" src="https://www.docker.com/wp-content/uploads/2022/03/vertical-logo-monochromatic.png"/>
      </a>
      <br />
      Docker
    </td>
  </tr>
</table>

## Key Features

- Orders
  - Create a orders with fields product name price and phone number

## Installation and launch method

Rename .env file, and set your variables for example:

```dotenv
MONGODB_URI=mongodb://root:password123@mongodb-primary:27017/
PORT=3000
RABBIT_MQ_URI=amqp://rabbitmq:5672
RABBIT_MQ_BILLING_QUEUE=billing
```

## Using Docker

Follow the command:

```shell
docker-compose up
# -d - For launch in the background
# --build - for build containers
```
