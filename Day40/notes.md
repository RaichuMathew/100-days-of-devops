# Day40 - Docker EXEC Operation

## Task:-
On App Server 3, access the running kkloud container and install apache2 using the apt package manager. Modify the Apache configuration to change the listening port from the default port 80 to port 8085 without binding it to any specific IP address, ensuring it listens on all interfaces. Restart or start the Apache service inside the container and verify that it is running properly. Ensure the kkloud container remains in a running state after completing the configuration.

## Purpose:-
This task validates container-level service configuration and management. Installing Apache enables web service functionality within the containerized environment. Changing the listening port to 8085 ensures customized service configuration without restricting network interfaces. Verifying the service status confirms proper deployment, while keeping the container running ensures application availability for further testing or integration.

