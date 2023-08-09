https://www.youtube.com/watch?v=Zc2mQSQXoS4

https://lucid.app/lucidchart/aadee838-9e81-4d05-94c3-565477a4e178/edit?viewport_loc=177%2C43%2C1705%2C886%2C0_0&invitationId=inv_ac85dd57-5db3-4142-b256-746f45a8d5b3

for admin side:
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
OR actually it automatically creates the table when running npm start because of createConnection of typeorm. 

To start developing, download typescript globally
  npm i typescript -g
  npm start
Watch ts files and automatically convert to js
  tsc -w

=============================================
for main (have to run this before admin to create the queues):
download mongodb
to start:
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