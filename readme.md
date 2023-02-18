desc author; desc book; desc card; desc student;desc transactions;


+---------+--------------+------+-----+---------+----------------+
| Field   | Type         | Null | Key | Default | Extra          |
+---------+--------------+------+-----+---------+----------------+
| id      | int          | NO   | PRI | NULL    | auto_increment |
| age     | int          | NO   |     | NULL    |                |
| country | varchar(255) | YES  |     | NULL    |                |
| name    | varchar(255) | YES  |     | NULL    |                |
| rating  | double       | NO   |     | NULL    |                |
+---------+--------------+------+-----+---------+----------------+
5 rows in set (0.00 sec)

+-----------+--------------+------+-----+---------+----------------+
| Field     | Type         | Null | Key | Default | Extra          |
+-----------+--------------+------+-----+---------+----------------+
| id        | int          | NO   | PRI | NULL    | auto_increment |
| genre     | varchar(255) | YES  |     | NULL    |                |
| issued    | bit(1)       | NO   |     | NULL    |                |
| name      | varchar(255) | YES  |     | NULL    |                |
| pages     | int          | NO   |     | NULL    |                |
| author_id | int          | YES  | MUL | NULL    |                |
| card_id   | int          | YES  | MUL | NULL    |                |
+-----------+--------------+------+-----+---------+----------------+
7 rows in set (0.00 sec)

+--------------------------+--------------+------+-----+---------+----------------+
| Field                    | Type         | Null | Key | Default | Extra          |
+--------------------------+--------------+------+-----+---------+----------------+
| id                       | int          | NO   | PRI | NULL    | auto_increment |
| card_status              | varchar(255) | YES  |     | NULL    |                |
| created_on               | datetime(6)  | YES  |     | NULL    |                |
| updated_on               | datetime(6)  | YES  |     | NULL    |                |
| student_variable_name_id | int          | YES  | MUL | NULL    |                |
+--------------------------+--------------+------+-----+---------+----------------+
5 rows in set (0.00 sec)

+-----------+--------------+------+-----+---------+----------------+
| Field     | Type         | Null | Key | Default | Extra          |
+-----------+--------------+------+-----+---------+----------------+
| id        | int          | NO   | PRI | NULL    | auto_increment |
| age       | int          | NO   |     | NULL    |                |
| country   | varchar(255) | YES  |     | NULL    |                |
| email     | varchar(255) | YES  | UNI | NULL    |                |
| mobile_no | varchar(255) | YES  |     | NULL    |                |
| name      | varchar(255) | YES  |     | NULL    |                |
+-----------+--------------+------+-----+---------+----------------+
6 rows in set (0.00 sec)

+--------------------+--------------+------+-----+---------+----------------+
| Field              | Type         | Null | Key | Default | Extra          |
+--------------------+--------------+------+-----+---------+----------------+
| id                 | int          | NO   | PRI | NULL    | auto_increment |
| fine               | int          | NO   |     | NULL    |                |
| is_issue_operation | bit(1)       | NO   |     | NULL    |                |
| transaction_date   | datetime(6)  | YES  |     | NULL    |                |
| transaction_id     | varchar(255) | YES  |     | NULL    |                |
| transaction_status | varchar(255) | YES  |     | NULL    |                |
| book_id            | int          | YES  | MUL | NULL    |                |
| card_id            | int          | YES  | MUL | NULL    |                |
+--------------------+--------------+------+-----+---------+----------------+
