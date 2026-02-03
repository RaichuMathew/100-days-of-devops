# Command Executed

## Check existing SSH directory on jump host (thor user)

ls -l .ssh/


## Generate SSH key pair for thor (no passphrase)
ssh-keygen -t rsa


## Verify SSH keys created on jump host
ls -l .ssh/

## Connect to App Server 1 using sudo user (first-time login)
ssh tony@stapp01


## Create SSH directory and authorized_keys file on App Server 1 (manual method)
mkdir .ssh
vi .ssh/authorized_keys

## Copy the key from jump host and paste in App server key file
vi .ssh/id_rsa.pub

## Exit from App Server 1
exit


## Verify password-less SSH access to App Server 1
ssh tony@stapp01


## Copy SSH public key to App Server 2 using ssh-copy-id
ssh-copy-id steve@stapp02

## Verify password-less SSH access to App Server 2
ssh steve@stapp02


## Copy SSH public key to App Server 3 using ssh-copy-id
ssh-copy-id banner@stapp03


## Verify password-less SSH access to App Server 3
ssh banner@stapp03


---

# Verification

* SSH key pair successfully generated for `thor` on the jump host
* Public key present in `authorized_keys` for all respective sudo users
* SSH access to all app servers works **without password prompts**
* Jump host can now be used for non-interactive automation scripts

---

# Result

Password-less SSH authentication from the jump host to all app servers using their respective sudo users has been successfully configured and val

