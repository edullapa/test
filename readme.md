# Teste 

- Na realização do teste, foi criado um banco com duas tabelas. A tabela product e category. A seguir são as instruções:

```bash
  $ mysql -u root -p
  mysql> CREATE DATABASE mall;
  mysql> show databases;
  // Criando as tabelas
  mysql> USE mall;
  mysql> drop table category;
  mysql> CREATE TABLE IF NOT EXISTS category(
       id INT(5) AUTO_INCREMENT PRIMARY KEY,
       name VARCHAR(20),
       description VARCHAR(50))ENGINE=MyISAM;

  mysql> drop table product;
  mysql> CREATE TABLE IF NOT EXISTS product(
       id INT(5) AUTO_INCREMENT PRIMARY KEY,
       name VARCHAR(20),
       description VARCHAR(50),
       price DECIMAL(10,2),
       category INT(5),
       FOREIGN KEY(category) REFERENCES category(id))ENGINE=MyISAM;
```

- Fim do teste.
