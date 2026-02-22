# Day41 :- Write a docker file

## Task:-
On App Server 3, create a Dockerfile at /opt/docker/Dockerfile using ubuntu:24.04 as the base image. Configure the Dockerfile to install apache2 and modify Apache configuration so it listens on port 8084 instead of the default port 80, without changing any other Apache settings such as document root. Ensure the container runs Apache in the foreground so the service remains active when the container starts.

## Purpose:-
This task enables creation of a custom Docker image tailored to application requirements. Using ubuntu:24.04 ensures a standardized base environment. Installing and configuring Apache to listen on port 8084 validates custom port configuration within containerized deployments while preserving default service structure. Running Apache in the foreground ensures proper container lifecycle management and service availability.

