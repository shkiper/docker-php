# Docker environment for php projects
Can be usefull for laravel / yii / lumen and other frameworks

This docker compose file setup three containers:
- web (nginx)
- app (php-fpm 7.1 v)
- database (mariadb latest)

## Instructions
- Put this files to your project
- Edit `docker-compose.yml`.
- Set mysql database name `MYSQL_DATABASE` and root password `MYSQL_ROOT_PASSWORD`
- Edit `nginx/vhost` for your project
- In database connection use host - `database` and user credentials from `docker-compose.yml`
- Run from console `docker-compose build` and wait...
- To start containers run `docker-compose up -d`