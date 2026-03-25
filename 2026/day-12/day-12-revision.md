# Revision 

##  Command
1. ps :- check all running process
2. systemctl status nginx :- it shows nginx is activate or deactivate
3. journalctl -u <service> :-it shows the logs and specific services

# file command
1. echo :- use for prin message
2. chmod :- use for change permission
3. chown :- change  owner
4. ls -l :- show all files and directory with owner,group , date,filename ,permission ,link
5. cp :- copying file to another one
6. mkdir :- make folder or directory

# create user
sudo useradd -m username
# set password
sudo passwd username
# change ownership 
sudo chown owner_name filename
# verify 
ls -l


#which command use most
I use touch,mkdir,cd,echo,mv,cp, and latest  is useradd,grupadd,chmod,chown,chgrp this command are use mostly because this is daily uses command and second one is i completed latest task so that are use his command

Service is healthy :- systemctl status servicename then check  ----> journalctl -u <service>

# safely change ownership :
sudo chown owner:group filename
# for directory
sudo chown -R owner:group directoryname

# I improve focus on next three days are hw to access and check  services ,log command




