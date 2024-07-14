## SQL

* It is a language used for interacting with RDBMS.
* Uses CRUD operations to communicate with database.

## QUERY

* Requests made to the DBMS for specific information.
* For eg: A google search is a query.

## SQL DATA TYPES

    DATA TYPE    |           DESCRIPTION
    ________________________________________________
      INT        |     Whole numbers eg: 5, 6, 7
     DECIMAL     |     Decimal values eg: 5.6, 7.9
    VARCHAR(n)   |     String of text of length 'n'
    DATETIME     |       YYYY-MM-DD HH:MM:SS
    BOOLEAN      |             0/1

## TYPES OF SQL COMMANDS:

1. DDL (Data Definition Language): Used for defining database schema.
      - CREATE: Create database or its objects (table, index, function, views, store procedure, and triggers)
                CREATE TABLE table_name (column1 data_type, column2 data_type, ...);
        
      - ALTER: Alter the structure of the database
                ALTER TABLE table_name ADD COLUMN column_name data_type;
        
      - DROP: Delete objects from the database
                DROP TABLE table_name;
        
      - TRUNCATE: Remove all records from a table, including all spaces allocated for the records are removed
                TRUNCATE TABLE table_name;
        
      - RENAME: Rename an object existing in the database
                RENAME TABLE old_table_name TO new_table_name;

2. DQL (Data Query Language): Used to retrieve data from the tables.
      - SELECT: It is used to retrieve data from the database
                SELECT column1, column2, ...FROM table_name<br>WHERE condition;

3. DML (Data Manipulation Language): Used to perform modifications in database.
      - INSERT: Insert data into a table 
                INSERT INTO table_name (column1, column2, ...) VALUES (value1, value2, ...);
   
      - UPDATE: Update existing data within a table
                UPDATE table_name SET column1 = value1, column2 = value2 WHERE condition;
        
      - DELETE: Delete records from a database table
                DELETE FROM table_name WHERE condition;

4. DCL (Data Control Language): Grant or revoke authorities from user.
      - GRANT: access user privileges to the DB.
                GRANT privilege_type [(column_list)] ON [object_type] object_name TO user [WITH GRANT OPTION];
        
      - REVOKE: revoke user privileges to the DB.
                REVOKE [GRANT OPTION FOR] privilege_type [(column_list)] ON [object_type] object_name FROM user [CASCADE];

5. TCL (Transaction Control Language): To manage transactions in database.
      - BEGIN TRANSACTION: Starts a new transaction
                BEGIN TRANSACTION [transaction_name];
        
      - COMMIT: This command is used to save the data permanently.
                COMMIT;
        
      - ROLLBACK: This command is used to get the data or restore the data to the last savepoint or last committed state.
                ROLLBACK;
        
      - SAVEPOINT: This command is used to save the data at a particular point temporarily, so that whenever needed can be rollback to that particular point.
                SAVEPOINT savepoint_name;
