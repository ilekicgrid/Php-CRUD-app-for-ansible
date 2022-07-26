# Web-Projekat

Name the database secondopinion.
Tables exist in sql format in a folder named sql.
For access change username and password in config.php and reg.php

Run it /// ansible-playbook -i inventory/hosts.yml deploy_the_app.yml -vv \\\  \n
IP of debian: 192:168:56:105  --- web server   \n
IP of centos: 192.168.56.104  --- database     \n
for direct ssh do: /// ssh-copy-id USER@HOST \\\  \n

Works on any machine. This was done in VirtualBox you need to setup network settings (NAT && hostOnly adapters). 
Setup sudoers file in debian (/ets/sudoers). 
Set up network configuration in CentOS.
if you want to secure your password use my existing file dbpassword.yml and do ansible-enxrypt dbpassword.yml. When you get the key copy paste on the 
location where the login_password was.
