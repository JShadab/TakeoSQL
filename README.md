# TakeoSQL
SQL stuff

What is DBMS (DataBase Management System):
-------------------------------------------
Network DBMS
Object Oriented DBMS
Distributed DBMS

Relational DBMS (RDBMS) OR SQL DBMS:
======================================
	1. MySQL
	2. Oracle
	6. MS SQLServer
	7. PostGRES SQL
	12. MariaDB	
	3. Amazon RDS
	5. IBM DB2
	6. MS SQLServer
	7. PostGRES SQL
	8. MS Acess
	9. Firebird
	10. h2
	11. GuptaSQL
	13. SQLite
	
-----------------------------------------------------
SQL:
-----
> SELECT * FROM <tableName>


NoSQL DBMS:
----------------
1. MongoDB
2. Cassandra
3. Elastic DB
4. GCP Big Tablex
5. Amazon DynamoDB


------------------------------------
SQL CMDs:
----------

1. To list all avaialable DBs:
---------------------------------
mysql> show databases;
  OR
mysql> show schemas;

2. To Create a new database:
------------------------------
mysql> create database takeo;
Query OK, 1 row affected (0.02 sec)

3. Switch to desired database:
----------------------------------
mysql> use takeo;
Database changed

4. To list all tables inside a database:
-------------------------------------------
mysql> show tables;
Empty set (0.06 sec)

5. How to create a table:
-------------------------------------------
mysql> CREATE TABLE employee (name VARCHAR(100), age INT, salary DOUBLE);


mysql> show tables;
+-----------------+
| Tables_in_takeo |
+-----------------+
| employee        |
+-----------------+
1 row in set (0.00 sec)

-----------------------------------------------
mysql> desc employee;
+--------+--------------+------+-----+---------+-------+
| Field  | Type         | Null | Key | Default | Extra |
+--------+--------------+------+-----+---------+-------+
| name   | varchar(100) | YES  |     | NULL    |       |
| age    | int          | YES  |     | NULL    |       |
| salary | double       | YES  |     | NULL    |       |
+--------+--------------+------+-----+---------+-------+
3 rows in set (0.01 sec)


mysql> SELECT * FROM employee;
Empty set (0.01 sec)



mysql> INSERT INTO employee (name, age, salary) VALUES ('Shadab Khan', 36, 1122.34);
Query OK, 1 row affected (0.01 sec)

mysql> SELECT * FROM employee;
+-------------+------+---------+
| name        | age  | salary  |
+-------------+------+---------+
| Shadab Khan |   36 | 1122.34 |
+-------------+------+---------+
1 row in set (0.00 sec)

===========================================================================================

Students
-----------------------
REGD_NO	NAME	BRANCH
0001	Ram	    CSE
0002	Hari	MECH
0003	Pradeep	EEE
0004	Deepak	ETC
-----------------------

1. Write down the SQL command which will show the Regd. No of Pradeep.
2. Write down the SQL command which will show the Name and Branch column.
3. Write a SQL command which will count the number of rows existing in STUDENT table.
4. I want to add another column in the STUDENT table as ”address”. How can I do that?


-----------------------------------------------------------
create table students (regd_no int, name varchar(25), branch varchar(5));

insert into students (regd_no, name, branch) values (0001, 'Ram', 'CSE');
insert into students  values (0002, 'Hari', 'MECH');
insert into students  values (0003, 'Pradeep', 'EEE');
insert into students  values (0004, 'Deepak', 'CIVIL');

select * from students;













