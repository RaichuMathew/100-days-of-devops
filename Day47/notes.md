# Day47 :- Create Docker Python App

## Task:-
On App Server 2, create a Dockerfile under /python_app using a Python base image. Configure the Dockerfile to copy the application source code, install dependencies from /python_app/src/requirements.txt, expose port 5003, and run server.py using CMD. Build a Docker image named nautilus/python-app using this Dockerfile. After building the image, create and run a container named pythonapp_nautilus, mapping container port 5003 to host port 8093. Verify the deployment by accessing the application using curl http://localhost:8093/ on App Server 2.

## Purpose:-
This task containerizes a Python application to ensure consistent deployment across environments. Installing dependencies from requirements.txt guarantees application compatibility. Exposing and mapping ports enables external access to the service. Building a custom image and deploying it as a container validates end-to-end Docker workflow, from image creation to runtime testing and service verification.
