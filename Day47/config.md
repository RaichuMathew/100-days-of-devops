# Commands Executed

## Connect to App server 2
ssh steve@stapp02

sudo su

## Nsavigate to the repo
cd /python_app/src/

cd .

vi Dockerfile

FROM python:3.10-slim

WORKDIR /app

COPY . .

RUN pip install -r src/requirements.txt

EXPOSE 5003

CMD ["python", "src/server.py"]

docker build -t nautilus/python-app .

docker run -d --name pythonapp_nautilus -p 8093:5003 nautilus/python-app

curl http://localhost:8093/
