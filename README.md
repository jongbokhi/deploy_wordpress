### Project Setup

This project implements a WordPress and MySQL environment using Kubernetes:

- **MySQL**  
  - Image: `mariadb:10.7`  
  - Port: `3306`  
  - Environment Variables:  
    - `MYSQL_DATABASE=wordpress`  
    - `MYSQL_ROOT_PASSWORD=password`  

- **WordPress**  
  - Image: `wordpress:5.9.1-php8.1-apache`  
  - Port: `80`  
  - Environment Variables:  
    - `WORDPRESS_DB_HOST=[wordpress host]`  
    - `WORDPRESS_DB_NAME=wordpress`  
    - `WORDPRESS_DB_USER=root`  
    - `WORDPRESS_DB_PASSWORD=password`  

