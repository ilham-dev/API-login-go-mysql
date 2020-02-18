# API-login-go-mysql
login API with bcrypt

# How to Run ?
#1.Create The Database with name go_api

#2. Create Table 
create table with name users

	CREATE TABLE `users` ( `id` INT(11) NOT NULL AUTO_INCREMENT , 
	`username` VARCHAR(50) NOT NULL , 
	`first_name` VARCHAR(200) NOT NULL , 
	`last_name` VARCHAR(200) NOT NULL , 
	`password` VARCHAR(120) NOT NULL , 
	`email`	   VARCHAR(200) NOT null ,
	PRIMARY KEY (`id`)) ENGINE = InnoDB;

#run
you should import the library first in terminal

	go get database/sql

	go get golang.org/x/crypto/bcrypt

	go get github.com/go-sql-driver/mysql
	go get github.com/kataras/go-sessions

### And here we go 
	go run main.go