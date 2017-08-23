# Ubuntu Cheat Sheet

## [Securing new server](https://www.linode.com/docs/security/securing-your-server)

On remote server install [Fail2Ban](http://www.fail2ban.org/wiki/index.php/Main_Page):`
sudo apt-get update && sudo apt-get install fail2ban`

Add folder for SSH keys:`
mkdir -p ~/.ssh && sudo chmod -R 700 ~/.ssh/
`

On your local machine create an SSH key pair if you haven't before:`
ssh-keygen -b 4096
`

Push SSH Key on local machine to remove server:`
cat ~/.ssh/id_rsa.pub | ssh ROOT@EXAMPLE.COM 'cat >> ~/.ssh/authorized_keys'
`

Verify SSH key connection, then disable password entry on remote server:`
vim /etc/ssh/sshd_config 
`

Then change `PasswordAuthentication` from `yes` to `no`, save the file, and finally restart SSH:`
sudo systemctl restart sshd
`

