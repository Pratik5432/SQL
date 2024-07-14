## SQL

* It is a language used for interacting with RDBMS.
* Uses CRUD operations to communicate with database.

## QUERY

* Requests made to the DBMS for specific information.
* For eg: A google search is a query.

## SQL DATA TYPES

    DATA TYPE             DESCRIPTION
      INT           Whole numbers eg: 5, 6, 7
     DECIMAL        Decimal values eg: 5.6, 7.9
    VARCHAR(n)      String of text of length 'n'
    DATETIME        YYYY-MM-DD HH:MM:SS
    BOOLEAN              0/1

## TYPES OF SQL COMMANDS:

1. DDL (Data Definition Language): Used for defining database schema.
      - CREATE
      - ALTER TABLE
      - DROP
      - TRUNCATE
      - RENAME

2. DQL (Data Query Language): Used to retrieve data from the tables.
      - SELECT 

3. DML (Data Manipulation Language): Used to perform modifications in database.
      - INSERT
      - UPDATE
      - DELETE

4. DCL (Data Control Language): Grant or revoke authorities from user.
      - GRANT: access user privileges to the DB.
      - REVOKE: revoke user privileges to the DB.

5. TCL (Transaction Control Language): To manage transactions in database.
      - COMMIT: This command is used to save the data permanently.
      - ROLLBACK: This command is used to get the data or restore the data to the last savepoint or last committed state.
      - SAVEPOINT: This command is used to save the data at a particular point temporarily, so that whenever needed can be rollback to that particular point.   
