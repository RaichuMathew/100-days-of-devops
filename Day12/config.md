# Commands Executed

## Initial Test from Jump Host (thor)
curl http://stapp01:3004
## Login to App Server 1
ssh tony@stapp01
sudo su
## Check Apache Status
systemctl status httpd
## Identify Port Conflict
netstat -tunlp --> sendmail is using the service 3004
## Modify Sendmail Port Configuration
cd /etc/
cd mail --> contains a config file named sendmail.cf
vi sendmail.cf --> Update the port from 3400 to 28
## Restart Apache Service
systemctl restart httpd
systemctl status httpd
## Re-test from Jump Host
Run curl http://stapp01:3004 in thor server and it throws an error, navigate back to app server 1
## Check Firewall Rules on App Server
iptables -L
Navigate back to thor and copy the ip address
## Allow Port 3004 from Jump Host IP
iptables -I INPUT -p tcp -s 172.16.238.3 --dport 3004 -j ACCEPT
service iptables save
service iptables restart
# Verification
curl http://stapp01:3004
Navigate to thor and try reaching out to it now

