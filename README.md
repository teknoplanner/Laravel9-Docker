# laravel9 Docker Compose

paket Fresh file laravel 9 with docker compose:
  - nginx:stable-alpine
  - mysql:latest
  - php8:stable-alpine

Docker-compose build nginx, mysql, and apche:
> docker-compose up -d --build

Add file .env

find file in "src"
> cd src

Copy file .env.example to .env

> cp env.example .env

Generate Key app laravel
> docker:compose run --rm artisan:key generate


