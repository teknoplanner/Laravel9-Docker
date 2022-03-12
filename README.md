# laravel9 Docker Compose

Fresh file laravel 9 with docker compose:
  - nginx:stable-alpine
  - mysql:latest
  - php8:stable-alpine
  - composer:latest
  - npm node:13.7
  - artisan


Docker-compose build nginx, mysql, and apche:
> docker-compose up -d --build

Add file .env, find file in folder "src"
> cd src

Copy file .env.example to .env

> cp env.example .env

#notes

Generate Key app laravel
> docker-compose run --rm artisan key:generate

run project on local browser
> localhost:8080





# notes

Laravel + docker Special command:
> docker-compose run --rm <"laravel command, for example migrate">

or
> docker-compose run --rm install <"package,  for example npm">

# Build container or delete

Build and running container
> docker-compose up -d --build

delete container
> docker-compose down





