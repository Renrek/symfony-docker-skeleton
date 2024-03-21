# basic-symfony-docker-template

## Setup
1. update git credentials in php/Dockerfile
1. docker compose up -d --build
1. docker-compose exec php bash
1. symfony check:requirements
1. symfony new .
1. verify site is operational at Http://localhost:8080

1. composer require --dev maker ormfixtures fakerphp/faker
1. composer require twig doctrine
1. cp .env .env.local
1. DATABASE_URL="mysql://root:secret@database:3306/symfony_docker?serverVersion=8.0"

### Notes
https://www.twilio.com/blog/get-started-docker-symfony



composer create-project symfony/skeleton:"7.0.*" .