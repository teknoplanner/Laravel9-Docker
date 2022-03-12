# laravel9 Docker Compose

paket Fresh file laravel 9 with docker compose:
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

Generate Key app laravel
> docker-compose run --rm artisan key:generate

run project on local browser
> localhost:8080

finish


notes: 

Laravel + docker Special commad:
> docker-compose run --rm <"laravel command, for example migrate">


