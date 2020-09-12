# WebCockpit readme

1. Run 'composer composer require firebase/php-jwt' inside included_files

2. **First create users in the "api_db" database**

        CREATE TABLE users (
            id int NOT NULL AUTO_INCREMENT, 
            username varchar(255) NOT NULL,
            firstname varchar(255) NOT NULL,
            lastname varchar(255) NOT NULL, 
            email varchar(255) NOT NULL, 
            password varchar(255) NOT NULL, 
            main_color varchar(255) NOT NULL,
            created datetime  DEFAULT CURRENT_TIMESTAMP NOT NULL, 
            modified timestamp DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP NOT NULL,
            PRIMARY KEY (id)
        );

3. **Connect DB to api using included_files/config/database.php file

