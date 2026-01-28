## Command Executed

# Connect to App Server 1
ssh banner@stapp01

# Switch to root user
sudo su -

# Edit SSH configuration
vi /etc/ssh/sshd_config
Update the configuration:- PermitRootLogin no

## Verification

# Check SSH configuration
sshd -T | grep permitrootlogin

## Output

permitrootlogin no
