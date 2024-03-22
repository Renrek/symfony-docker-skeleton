# symfony-docker-skeleton

## Quick Setup
1. docker compose up -d --build
1. docker compose exec php bash
1. composer create-project symfony/skeleton .
1. cp .env .env.local

## Optional 
- Alternate syntax: composer create-project symfony/skeleton:"7.0.*" .
- composer require twig doctrine
- composer require --dev maker ormfixtures fakerphp/faker

## Notes
1. Always run composer commands from within container
1. Site can be found at: Http://localhost:8080