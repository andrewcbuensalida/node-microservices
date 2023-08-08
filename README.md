https://www.youtube.com/watch?v=Zc2mQSQXoS4

Create a new database in mysql workbench
click create a new schema
schema name = yt_node_admin
create product table
  CREATE TABLE `yt_node_admin`.`product` (
  `id` INT NOT NULL AUTO_INCREMENT,
  `title` VARCHAR(45) NULL,
  `image` VARCHAR(45) NULL,
  `likes` INT NULL DEFAULT 0,
  PRIMARY KEY (`id`));

OR with gui

To start developing, download typescript globally
  npm i typescript -g
  npm start
Watch ts files and automatically convert to js
  tsc -w

=============================================
run rabbitmq container
   docker run -d --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.12-management

add -d to make it detached

check if it's running
  docker ps -a

To run hello_world/send.js
  node send
same for receive.js

Go to rabbitmq management console, In browser
  http://localhost:15672/
Username and password is "guest"