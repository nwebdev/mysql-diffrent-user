# mysql-diffrent-user

# Create a new MySQL User Account

     CREATE USER 'newuser'@'%' IDENTIFIED BY 'user_password';
     CREATE USER 'newuser'@'localhost' IDENTIFIED BY 'user_password';
     CREATE USER 'newuser'@'10.8.0.5' IDENTIFIED BY 'user_password';

# Grant Privileges to a MySQL User Account

The most commonly used privileges are:

    ALL PRIVILEGES – Grants all privileges to a user account.
    CREATE – The user account is allowed to create databases and tables.
    DROP - The user account is allowed to drop databases and tables.
    DELETE - The user account is allowed to delete rows from a specific table.
    INSERT - The user account is allowed to insert rows into a specific table.
    SELECT – The user account is allowed to read a database.
    UPDATE - The user account is allowed to update table rows.
    
syntax     

    GRANT CREATE, DELETE, INSERT, SELECT, UPDATE  ON database_name.table_name TO 'database_user'@'localhost';
    
    GRANT ALL PRIVILEGES ON database_name.* TO 'database_user'@'localhost';

    SHOW GRANTS FOR 'database_user'@'localhost';

# Revoke Privileges from a MySQL User Account

    REVOKE ALL PRIVILEGES ON database_name.* FROM 'database_user'@'localhost';

# Remove an Existing MySQL User Account

    DROP USER 'user'@'localhost'
