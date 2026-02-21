# Day37 :- Copy file to docker

## Task:-
On App Server 1, copy the encrypted file /tmp/nautilus.txt.gpg from the Docker host into the running container named ubuntu_latest, placing it inside the container at /tmp/. Ensure the file is transferred without modification and verify its presence inside the container after the copy operation.

## Purpose:-
This task validates secure file transfer between the Docker host and a running container without altering file integrity. Copying the encrypted file as-is ensures confidentiality is preserved, while verification confirms successful data movement into the container environment for further controlled processing.

