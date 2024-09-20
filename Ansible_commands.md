# yum install ansible -y --> to install ansible
# ansible --version --> To check ansible version
# ansible -i inventory.ini all -e ansible_user=centos ansible_password=DevOps321 -m ping ----> To chech connections
# ansible-playbook -i inventory.ini all -e ansible_user=centos ansible_password=DevOps321 mongodb.yaml

$$ --> display script PID
$? --> exit status
$! --> PID of last command running in the bachgrounf
# ansibel-playbook -i inventory -e ansible_user=centos -e ansibel_password=DevOps321 &  ---> It is running in the background
# nohup ansibel-playbook -i inventory -e ansible_user=centos -e ansibel_password=DevOps321 & >> /dev/null --> if you don't want running output in consile, Run this command
# tail -f nohup.out --> output stored here
Shell vs Command:-
-----------------
Shell:- It is like you login inside the server and run the command. env variable and redirections will work
Command:- It is like running command from outside. Redirection and env varaibles will not work.

DRY --> Don,t repeat your self
We created a function kept code inside. Whenever you want call the finction
Reduce duplicate code and a central place to change.

# ansible-playbook -i inventory.ini -e ansible_user=centos -e ansible_password=DevOps321 -e components=mongodb main.yaml --> Ansible roles 

# cp /etc/ansible/ansible.cfg test/
# export ANSIBLE_CONFIG=/home/centos/test/ansible.cfg --> to set the variable
# unset ANSIBLE_CONFIG ---> unset env variable
#cp /etc/ansible/ansible.cfg ansible.cfg
# cat ansible.cfg 
# ansible-config init --disabled > ansible.cfg --->To generate an example config file (a "disabled" one with all default settings, commented out):

Calalogue service l;ocation
---------------------------
# cat /etc/systemd/system/catalogue.service





