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

## Basic-Architecture (tree)
********
src  
    ├───controllers  # functions to connect routes to db operations   
    ├───db           # db connections and model definations  
    ├───public       # html/css/js file for static part of site   
    ├───routes       # express middlewares (routes wise)  
    └───utils        # functions to connect to db operations   

*****