# Commands Executed
## Install Tomcat on App Server 3
ssh banner@stapp03

sudo yum install -y tomcat
## Configure Tomcat to Run on Port 5004
sudo vi /etc/tomcat/server.xml
Update Connector port from 8080 to 5004

## Start and Enable Tomcat Service
sudo systemctl start tomcat
sudo systemctl enable tomcat

## Copy ROOT.war from Jump Host to App Server(Run in jumphost)
scp /tmp/ROOT.war banner@stapp03:/home/banner

## Deploy ROOT.war in Tomcat
sudo mv /tmp/ROOT.war /usr/share/tomcat/webapps/
sudo chown tomcat:tomcat /usr/share/tomcat/webapps/ROOT.war

##  Restart Tomcat to Apply Deployment
sudo systemctl restart tomcat
# Verification 
curl http://stapp03:5004
