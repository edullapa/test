# Spring Boot application 

It's a sampling of how Spring Boot helps you accelerate and facilitate application development.
The additional softwares are used ender development:
-**MySQL**: Open-source relational database management system used to development project. You need to create a MySQL database named **mall** and you have registered a connection for in the Eclipse IDE. The table data is contained as follow: 

```bash
  $ mysql -u root -p
  mysql> CREATE DATABASE mall;
  mysql> SHOW DATABASES;
  // Table data
  mysql> USE mall;
  mysql> DROP TABLE category;
  mysql> CREATE TABLE IF NOT EXISTS category(
       id INT(5) AUTO_INCREMENT PRIMARY KEY,
       name VARCHAR(20),
       description VARCHAR(50))ENGINE=MyISAM;

  mysql> DROP TABLE product;
  mysql> CREATE TABLE IF NOT EXISTS product(
       id INT(5) AUTO_INCREMENT PRIMARY KEY,
       name VARCHAR(20),
       description VARCHAR(50),
       price DECIMAL(10,2),
       category INT(5),
       FOREIGN KEY(category) REFERENCES category(id))ENGINE=MyISAM;
```

-**Eclipse IDE**.
-**Maven**.