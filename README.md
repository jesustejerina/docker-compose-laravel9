# docker-compose-laravel9
<b>Workspace to Laravel 9 projects.</b><br>
Include container nginx, php, mariadb, phpmyadmin<br><br>
Edit docker-compose.yml for mariadb service and update: MARIADB_USER, MARIADB_DATABASE, MARIADB_ROOT_PASSWORD.<br>
Create two folders: src and mariadb<br>
Inside folder Mariadb, will store the data generated.<br>
The laravel 9 project, you have to will create inside the src folder.<br>
Inside src folder (terminal), run <b>docker-compose up -d</b> for open the workspace-containers.<br>
Open terminal of php container and execute the command COMPOSER CREATE-PROJECT LARAVEL/LARAVEL <b>.</b> 9.* (note the dot. That indicates that the project will not generate a folder name and version laravel is 9).<br>
Inside container php run: chown -R www-data:www-data storage<br>
Open your host navigator and go to http://localhost:8888 for show laravel welcome blade.<br><br>
<b>php container include:</b><br>
Image base php:8.1.15-fpm-alpine3.17<br>
composer 2.53,<br>
node 18.12.1,<br>
npm 9.1.2.<br><br><br>
For view php extension run:<br>
docker run -it --rm jesusitodocker/for-laravel9:1.0 php -m<br><br>
<b>USING VISUAL STUDIO CODE</b><br>
Open VS Code and install <b> DEV CONTAINER (microsoft)</b> extension.<br>
Attach VS Code to php container.<br>
Open folder /var/www/html<br>
Edit .env file for database configuration DB_HOST=mariadb and other var<br>
<b>All the laravel commands, you can run directly from the PHP container terminal.</b><br>
Execute migration.<br>
And Ready to code.
<br><br><b>Thanks...</b>

