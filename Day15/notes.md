# Day15

## Task:

Connect to App Server 2 and prepare it for application deployment by:

Installing and configuring nginx.

Enabling and starting the nginx service.

Moving the self-signed SSL certificate (/tmp/nautilus.crt) and key (/tmp/nautilus.key) to an appropriate secure location inside the nginx directory.

Configuring nginx to use the moved SSL certificate and key for HTTPS on port 443.

Creating an index.html file with the content Welcome! under the nginx document root (/usr/share/nginx/html).

Testing HTTPS connectivity from the jump host using curl -Ik https://<app-server-ip>/.

## Purpose:

Ensure App Server 2 is fully configured with nginx and secured using the provided SSL certificate so that the application can be hosted over HTTPS, verified by successfully accessing it from the jump host.
