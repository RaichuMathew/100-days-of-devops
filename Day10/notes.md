#Day10
## Task:
Create a bash script on App Server 3 to take a backup of the beta website
and store it locally as well as on the Nautilus Backup Server.

## Purpose:
The production team requires an automated and reusable backup solution
for the static beta website. The script creates a zip archive of the
/var/www/html/beta directory, stores it temporarily on the local server,
and securely copies it to the central Nautilus Backup Server. Passwordless
SSH authentication ensures the script runs non-interactively, and the
solution follows security best practices by avoiding sudo usage inside
the script.

