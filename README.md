# docker-compose-laravel9
<b>Workspace to Laravel 9 projects.</b><br>
Include container nginx, php, mariadb, phpmyadmin<br><br>
Create two folders: src and mariadb<br>
Inside folder Mariadb, will store the data generated.<br>
The laravel 9 project, you have to will create inside the src folder. Get in terminal of php container and execute the command COMPOSER CREATE-PROJECT LARAVEL/LARAVEL . (note the dot at the end. That indicates that the project will not generate a folder name).<br><br>
<b>php container include:</b><br>
Image base php:8.1.15-fpm-alpine3.17<br>
composer 2.53,<br>
node 18.12.1,<br>
npm 9.1.2.<br><br><br>
For view php extension run:<br>
docker run -it --rm jesusitodocker/for-laravel9:1.0 php -m<br><br>
Thanks...

