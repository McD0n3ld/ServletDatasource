Creacion usuario

CREATE USER 'raul'@'localhost' IDENTIFIED BY '1234';
mysql –u raul –p 1234
create database midatasource;
use midatasource;

Creación de la tabla de SQL necesaria:

CREATE TABLE IF NOT EXISTS `employee` (
  `emp_id` int auto_increment,
  `emp_name` varchar(255) NOT NULL,
  `salary` double DEFAULT NULL,
  `dept_name` varchar(255) DEFAULT NULL,
  PRIMARY KEY (`emp_id`)
) ;

Insertar valores:

INSERT INTO employee VALUES(1, 'raul',5000,'jaja');

maven install

Correr el TOMCAT

http://localhost:8080/ServletDatasource/EmployeeServlet