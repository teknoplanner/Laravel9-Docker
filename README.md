# laravel9 Docker Compose

paket Fresh file laravel 9 with docker compose:
  - nginx:stable-alpine
  - mysql:latest
  - php8:stable-alpine

Docker-compose build nginx, mysql, and apche:
> docker-compose up -d --build

Copy file .env.example to .env
find file in "src"
> cd src
> cp env.example .env

Generate Key app laravel
> docker:compose run --rm artisan:key generate


