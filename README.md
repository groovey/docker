# Docker

The most commonly used docker services.

## Start

    docker-compose up -d

## Mysql 8 create a user

    docker-compose exec mysql mysql -u root -p

    // Create user
    CREATE USER 'web'@'%' IDENTIFIED WITH mysql_native_password BY 'webdevel';
    GRANT ALL PRIVILEGES ON *.* TO 'web'@'%' WITH GRANT OPTION;
    FLUSH PRIVILEGES;

## Mysql show users

    use mysql;
    SELECT user FROM user;
    SELECT 
        user, 
        host, 
        account_locked, 
        password_expired
    FROM
        user;

## Phpmyadmin

    http://localhost:8080/
    server: mysql
    username: root
    password: webdevel  

## Connect via Mysql Workbench

    hostname: 127.0.0.1
    port: 3306
    username: root
    password: webdevel 
