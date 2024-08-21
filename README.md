Using ansible this hands on project shows :
 - how to Create a user with Password 
 - Create a group and add user to the group.
 - Clone a repo of your choice and user couldn’t have acces into the clone repo
 - and giving the user permission to access into the clone repo

STEPS
 - create 2 Ec2 instances and use one as the control node and manage node respectively
 - ssh into the control node
 - install ansible on the control node
 - edit your default hosts file by sudo into it "sudo vim /etc/ansible/hosts/"
 - add your Ec2 instances public ip address of the manage node   
 - create ansible playbook file in yaml
 - ping the default hosts file to know the status,it must give you a "ping-pong" result "ansible name-of-hosts -m ping --private-key /path-to-ur-key/app-key.pem"
 - run your ansible playbook file to carry the task on the manage node "ansible-playbook playbook-name.yaml --private-key /path-to-ur-key/app-key.pem"
