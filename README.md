# Laravel9 Docker Compose

Fresh file laravel 9 with docker compose:
  - nginx:stable-alpine
  - mysql:latest
  - php8:stable-alpine
  - composer:latest
  - npm node:13.7
  - artisan



Docker-compose build nginx, mysql, and php8:
> docker-compose up -d --build

Add file .env, find file in folder "src"
> cd src

Copy file .env.example to .env
> cp .env.example .env

Update folder /vendor and Auto load
> docker-compose run --rm composer update

Generate Key app laravel
> docker-compose run --rm artisan key: generate

run project on local browser
> localhost:8080


#  Add Vue.js

update Laravel/ui, composer.json
> docker-compose run --rm composer require laravel/ui

install vue to project
>  docker-compose run --rm artisan ui vue 

npm installation
>  docker-compose run --rm npm install 

run development
> docker-compose run --rm npm run dev  

running npm watch
>  docker-compose run --rm npm run watch-poll

# add tailwind
problem : npx 

> USE CDN: https://tailwindcss.com/docs/installation/play-cdn


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







