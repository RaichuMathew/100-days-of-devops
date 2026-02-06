# Day09
## Task:
Fix MariaDB service issue on the database server (stdb01).

## Purpose:
The MariaDB service was failing to start because the required
data directory (/var/lib/mysql) was missing. MariaDB depends on
this directory to store database files and cannot run without it.
Creating the directory and assigning correct ownership (mysql:mysql)
restores proper access, allowing the MariaDB service to start
successfully and re-establish database connectivity for the application.

