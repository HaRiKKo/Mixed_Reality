# Mixed_Reality
Scholarship mixed reality project. Unity and Vuforia maze game.  

# Prerequisites
- OpenJDK 8
- the JDBC instance: MySQL **AND** PastgreSQL

# First start 
Clone the repot in your local environment. As example, you can use the command `git clone` with the SSH key. 
Then you connect to MySQL and PastgreSQL. 

For MySQL:
  You create the user `myusr` with the password `Password1!`, and you can grant him the rights on the already existing databases. 
```
  CREATE USER 'myuser'@'localhost' IDENTIFIED BY 'Password1!';
  GRANT ALL PRIVILEGES ON *.* TO 'myuser'@'localhost';
  FLUSH PRIVILEGES;
```
  Next, you log in with your new account and you create the database `customer` with it.
```
  mysql -u myuser -p
  CREATE DATABASE customer;
```
For PostgreSQL:
  You realized the same operation that mention above. You create the user `myusr` with the password `Password1!`. You need to grant the login right and create database privileges.
  ```
    CREATE USER myuser WITH ENCRYPTED PASSWORD 'Password1' CREATEDB LOGIN;
  ```
  Then you create the database `orders` with `myuser` as owner. Then, you assign all priviledges to `myuser` on this database.
  ```
  CREATE DATABASE orders OWNER myuser;
  GRANT all privileges ON DATABASE orders TO myusr;
  ```

