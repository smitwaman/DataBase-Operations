Cheat sheet for common SQL database operations:

1. **Create a Database:**
   ```sql
   CREATE DATABASE database_name;
   ```

2. **Use a Database:**
   ```sql
   USE database_name;
   ```

3. **Create a Table:**
   ```sql
   CREATE TABLE table_name (
       column1 datatype,
       column2 datatype,
       ...
   );
   ```

4. **Insert Data into a Table:**
   ```sql
   INSERT INTO table_name (column1, column2, ...)
   VALUES (value1, value2, ...);
   ```

5. **Select Data from a Table:**
   ```sql
   SELECT column1, column2, ...
   FROM table_name
   WHERE condition;
   ```

6. **Update Data in a Table:**
   ```sql
   UPDATE table_name
   SET column1 = value1, column2 = value2, ...
   WHERE condition;
   ```

7. **Delete Data from a Table:**
   ```sql
   DELETE FROM table_name
   WHERE condition;
   ```

8. **Add a Column to a Table:**
   ```sql
   ALTER TABLE table_name
   ADD column_name datatype;
   ```

9. **Modify a Column in a Table:**
   ```sql
   ALTER TABLE table_name
   MODIFY column_name datatype;
   ```

10. **Drop a Column from a Table:**
    ```sql
    ALTER TABLE table_name
    DROP COLUMN column_name;
    ```

11. **Drop a Table:**
    ```sql
    DROP TABLE table_name;
    ```

12. **Create an Index:**
    ```sql
    CREATE INDEX index_name
    ON table_name (column1, column2, ...);
    ```

13. **Drop an Index:**
    ```sql
    DROP INDEX index_name
    ON table_name;
    ```

14. **Count the Number of Rows in a Table:**
    ```sql
    SELECT COUNT(*)
    FROM table_name;
    ```

15. **Group Data and Perform Aggregation:**
    ```sql
    SELECT column1, COUNT(*)
    FROM table_name
    GROUP BY column1;
    ```

16. **Join Tables:**
    ```sql
    SELECT *
    FROM table1
    INNER JOIN table2 ON table1.column = table2.column;
    ```

17. **Create a View:**
    ```sql
    CREATE VIEW view_name AS
    SELECT column1, column2, ...
    FROM table_name
    WHERE condition;
    ```

18. **Grant Privileges:**
    ```sql
    GRANT privilege_name
    ON database_name.table_name
    TO user_name;
    ```

19. **Revoke Privileges:**
    ```sql
    REVOKE privilege_name
    ON database_name.table_name
    FROM user_name;
    ```

20. **Backup and Restore a Database:**
    - Backup: `mysqldump -u username -p database_name > backup_file.sql`
    - Restore: `mysql -u username -p database_name < backup_file.sql`

Feel free to refer to this cheat sheet whenever you need to perform SQL database operations
