# MySQL Command

## Login
```sql
mysql -u root -p
```
## List all Databases
```sql
show databases;
```
## Select database
```sql
use databaseName;
```
## List all tables
```sql
show tables;
```
## Create Database 
```sql
CREATE DATABASE mydatabase CHARACTER SET utf8 COLLATE utf8_general_ci;
```
## Dump Database with store procedure and functions
```sql
mysqldump --routines -u root -p db_name > name.sql
```
## Dump Database with store procedure and functions as gzip
```
mysqldump --routines -u root -p db_name | gzip > name.sql.gz
```
## Restore Database
```sql
mysql -u root -p db_name < name.sql
```
## Restore Database from gzip
```sql
gunzip < name.sql.gz | mysql -u root -p db_name
```
## List store procedure 
```sql
SHOW PROCEDURE STATUS WHERE db = 'db_name';
```
## List functions
```sql
SHOW FUNCTION STATUS WHERE db = 'db_name';
```
