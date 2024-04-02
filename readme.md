//Create Database
CREATE DATABASE mydb;

//use database
USE mydb;

//Create Table
CREATE TABLE user
(
id int unsigned,
name varchar(20),
email varchar(50),
password varchar(100),
phone varchar(15),
address text
)

//Add Rows
INSERT INTO user
(id,name,email,password,phone,address)
VALUES
(1, "shardul", "shardul@gmail.com", "password", "7894561237", "dummy address")

//Add Mutliple rows at once
INSERT INTO user
(id,name,email,password,phone,address)
VALUES
(1, "shardul", "shardul@gmail.com", "password", "7894561237", "dummy address"),
(2, "shardul2", "shardul2@gmail.com", "password", "7894561237", "dummy address2"),
(3, "shardul3", "shardul3@gmail.com", "password", "7894561237", "dummy address3")

//Fetch data from table
SELECT * FROM user; //fetch all data with all columns
SELECT name, email FROM user; //fetch specific columns data
SELECT name AS 'User Name' FROM user; //To give alias to column

//Fetch data using WHERE clause to use filter the data
SELECT id, name AS "User Name", email 
FROM user 
WHERE name = "shardul"  //conditions-> = , != , >= , <= , > , <

//Contraints is used to validate the data

# sql-queries
