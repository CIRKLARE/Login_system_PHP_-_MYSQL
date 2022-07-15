# Login system using PHP and MYSQL
this is vulnerable website



sudo apt install mariadb-server
systemctl start mariadb
systemctl start mysql
mysql -u root -p
create database test_db;
use test_db;

CREATE TABLE users (
  id int(11) NOT NULL,
  user_name varchar(255) NOT NULL,
  password varchar(255) NOT NULL,
  name varchar(255) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

INSERT INTO users (id, user_name, password, name) VALUES
(1, 'admin', 'qwerty', 'admin'),
(2, 'elias', '123', 'Elias'),
(3, 'john', 'abc', 'John');


ALTER TABLE users
  ADD PRIMARY KEY (id);


ALTER TABLE users
  MODIFY id int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=3;
COMMIT;



# to add new user

INSERT INTO users (id, user_name, password, name) VALUES (4, 'tom', 'password', 'Tom');



sudo php -S 0.0.0.0:80








