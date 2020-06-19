# Layout-for-SM-

## Database-setup (using mysql2 with sequalize)

**********
shell
********

mysql -u root -p
create database smdb;
create user smuser identified with mysql_native_password by 'smpass';
grant all privileges on smdb.* to smuser ; 
flush privileges;
 
*******
