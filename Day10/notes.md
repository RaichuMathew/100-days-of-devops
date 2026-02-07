## Task:
Resolve MariaDB service failure on the database server (stdb01).

## Purpose:
The MariaDB service was failing to start because required directories
used by the database were missing or misconfigured. MariaDB depends on
/var/lib/mysql for storing database files and /var/run/mysqld for
creating runtime socket and PID files. Since these directories were
absent or inaccessible, the MariaDB daemon exited immediately with
status=1. Creating the directories and assigning correct ownership
(mysql:mysql) restored proper access, allowing the MariaDB service to
start successfully and re-enable application connectivity to the
database.

