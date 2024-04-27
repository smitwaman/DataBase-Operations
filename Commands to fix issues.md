Common database problems and the commands needed for troubleshooting:

1. **Performance Issues:**
   - Identify slow queries:
     ```sql
     EXPLAIN SELECT * FROM table_name WHERE condition;
     ```
   - Monitor database activity:
     ```sql
     SHOW PROCESSLIST;
     ```

2. **Connection Errors:**
   - Check network connectivity:
     ```
     ping database_server_ip
     ```
   - Verify database server status:
     ```
     systemctl status mysql
     ```

3. **Deadlocks:**
   - Analyze deadlock logs:
     ```sql
     SHOW ENGINE INNODB STATUS;
     ```

4. **Data Corruption:**
   - Perform integrity checks:
     ```sql
     CHECKTABLE table_name;
     ```

5. **Disk Full Errors:**
   - Free up disk space:
     ```
     sudo rm -rf /path/to/unneeded/files
     ```

6. **Security Breaches:**
   - Update database software:
     ```
     sudo apt update && sudo apt upgrade
     ```
   - Monitor database activity:
     ```sql
     SELECT * FROM mysql.general_log WHERE event_time > NOW() - INTERVAL 1 DAY;
     ```

7. **Replication Lag:**
   - Monitor replication lag:
     ```sql
     SHOW SLAVE STATUS\G;
     ```

8. **Backup Failures:**
   - Check backup schedules:
     ```
     crontab -l
     ```

9. **Query Locking and Blocking:**
   - Identify blocking queries:
     ```sql
     SHOW PROCESSLIST;
     ```

10. **Resource Contention:**
    - Monitor database resource usage:
      ```
      htop
      ```
      
Remember to adjust these commands according to your specific database management system and operating system. Always exercise caution when executing commands, especially those that can impact system configuration or data integrity
