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


