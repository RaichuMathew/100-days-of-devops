# Day44 :- Docker Compose
## Task:-
On App Server 3, create a Docker Compose file at /opt/docker/docker-compose.yml. Configure it to deploy a service using the latest httpd image and ensure the container name is set to httpd. Map host port 3000 to container port 80. Mount the host directory /opt/dba to the container path /usr/local/apache2/htdocs without modifying any existing data. Use docker compose to bring up the service and ensure the container remains in a running state.

##Purpose:-
This task provisions a containerized Apache HTTP server environment using Docker Compose for structured deployment. Port mapping enables external access to the web service via host port 3000. Volume mapping ensures static website content from /opt/dba is served by the container without altering existing data. Using Docker Compose standardizes service configuration and supports consistent application hosting.

