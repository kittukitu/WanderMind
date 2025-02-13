show tables;
+-----------------+
| Tables_in_brain |
+-----------------+
| otps            |
| users           |
+-----------------+
2 rows in set (0.04 sec)

mysql> desc otps;
+------------+--------------+------+-----+---------+----------------+
| Field      | Type         | Null | Key | Default | Extra          |
+------------+--------------+------+-----+---------+----------------+
| id         | int          | NO   | PRI | NULL    | auto_increment |
| email      | varchar(255) | NO   |     | NULL    |                |
| otp        | varchar(6)   | NO   |     | NULL    |                |
| expires_at | datetime     | NO   |     | NULL    |                |
+------------+--------------+------+-----+---------+----------------+
4 rows in set (0.05 sec)

mysql> desc users;
+----------+--------------+------+-----+---------+----------------+
| Field    | Type         | Null | Key | Default | Extra          |
+----------+--------------+------+-----+---------+----------------+
| id       | int          | NO   | PRI | NULL    | auto_increment |
| username | varchar(255) | YES  |     | NULL    |                |
| email    | varchar(255) | NO   | UNI | NULL    |                |
| password | varchar(255) | NO   |     | NULL    |                |
| phone    | varchar(20)  | YES  |     | NULL    |                |
| location | varchar(255) | YES  |     | NULL    |                |
| gender   | varchar(20)  | YES  |     | NULL    |                |
| role     | varchar(20)  | YES  |     | user    |                |
+----------+--------------+------+-----+---------+----------------+
