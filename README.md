# symfony-docker-skeleton

## Quick Setup
1. docker compose up -d --build
1. docker compose exec php bash
1. composer create-project symfony/skeleton .
1. composer require twig doctrine
1. composer require --dev maker
1. cp .env .env.local
1. Add ```DATABASE_URL="mysql://root:secret@database:3306/symfony_docker"``` to .env.local

## Optional 
- For Production comment out database container in compose file.
- Alternate syntax: composer create-project symfony/skeleton:"7.0.*" .
- composer require --dev maker ormfixtures fakerphp/faker

## Notes
- Always run composer commands from within container
- Site can be found at: Http://localhost
- php bin/console make:entity {modelName}
- php bin/console make:migration
- php bin/console doctrine:migrations:migrate