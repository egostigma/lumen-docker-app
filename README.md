# lumen-docker-app

## Usage

Install Composer:
- `docker run --rm -v $(pwd):/app composer install`

Start docker image:
- `docker-compose up -d`

Run npm commands:
- `docker-compose exec app npm install`
- `docker-compose exec app npm run dev`

Run artisan commands:
- `docker-compose exec app php artisan key:generate`
- `docker-compose exec app php artisan config:cache`
- `docker-compose exec app php artisan migrate`

(Optional) Set permissions on the project directory so that it is owned by your non-root user:
- `sudo chown -R $USER:$USER ./`

## TODO
Persist MySQL local data
