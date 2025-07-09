##How to run the migration and other commands


# Run this command to create a laravel project on source folder
docker compose run -d --build --rm composer create-project --prefer-dist laravel/laravel .


# To run all the services use 
docker compose up services


# To run one by one  services use 
docker compose up service-name

## To go inside the php container and run any artisan command use this 
docker-compose exec 

# To run artisan command use this 
docker-compose exec php php artisan migrate

# After cloning
docker-compose up -d --build
docker-compose exec php composer install
docker-compose exec php php artisan migrate
