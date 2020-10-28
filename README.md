### Docker Common

The Most commonly used docker services

### Start

    $ docker-compose up -d

### Mysql 8 create a user


    docker-compose exec mysql mysql -u root -p

    // Create user
    CREATE USER 'web'@'%' IDENTIFIED WITH mysql_native_password BY 'webdevel';
    GRANT ALL PRIVILEGES ON *.* TO 'web'@'%' WITH GRANT OPTION;
    FLUSH PRIVILEGES;

### Phpmyadmin

    http://192.168.99.101:8080/
    server: mysql
    username: root
    password: webdevel


