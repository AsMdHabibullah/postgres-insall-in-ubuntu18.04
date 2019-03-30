============================================================
# Install and Use PostgreSQL on Ubuntu 18.04
Also we can setup PostgreSQL for python django framework.
============================================================

First we need to install PostgreSQL & setup by the help of Ubuntu terminal & command.

```
Start:
sudo aot update
sudo apt install postgresql postgresql-contrib
Installation done.
So Now..............command is................
service postgresql
service postgresql status
sudo su postgres
psql
postgres=# \l

And now show the defoult database like this.
postgres=# \l
                                  List of databases
   Name    |  Owner   | Encoding |   Collate   |    Ctype    |   Access privileges   
-----------+----------+----------+-------------+-------------+-----------------------
 postgres  | postgres | UTF8     | en_US.UTF-8 | en_US.UTF-8 | 
 template0 | postgres | UTF8     | en_US.UTF-8 | en_US.UTF-8 | =c/postgres          +
           |          |          |             |             | postgres=CTc/postgres
 template1 | postgres | UTF8     | en_US.UTF-8 | en_US.UTF-8 | =c/postgres          +
           |          |          |             |             | postgres=CTc/postgres
(3 rows)

postgres=# 

And now show the all user like this.
postgres=# \du
                                   List of roles
 Role name |                         Attributes                         | Member of 
-----------+------------------------------------------------------------+-----------
 postgres  | Superuser, Create role, Create DB, Replication, Bypass RLS | {}

postgres=# 

Now we can change our defoult password by this command.

ALTER USER postgres WITH PASSWORD '12345678089865';

if we enter then show like this.

ALTER ROLE

Now we can create new user and password by this command.

CREATE USER user_1 WITH PASSWORD '12344567877';

if we enter then show like this.
CREATE ROLE


Now again check the total user by this command

postgres=# \du
                                      List of roles
   Role name    |                         Attributes                         | Member of 
----------------+------------------------------------------------------------+-----------
 user_1 |                                                            | {}
 postgres       | Superuser, Create role, Create DB, Replication, Bypass RLS | {}

postgres=# 


We can also delate the user by this command.
postgres=# DROP USER user_1;

if we enter then show like this.
DROP ROLE


Now again we can check the total user by this command.
postgres=# \du
                                   List of roles
 Role name |                         Attributes                         | Member of 
-----------+------------------------------------------------------------+-----------
 postgres  | Superuser, Create role, Create DB, Replication, Bypass RLS | {}

postgres=# 

Also we can use (man psql) command for postgresql help.

For quite command install
\q
```

```
Thanks
AsMd Habibullah
Yunnan University
Department: Computer Science & Technology.
```
