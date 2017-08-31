## Mysql Server Provisioning in EC2 using Ansible 

OBJECTIVE: Create an Ansible playbook that takes in an input of a number, and launch/spin-up that number of AWS EC2 instances in the default VPC with MySQL installed and all instances updated.


**Usage:**

Create a variables file using *ec2_vars/sample.yml* as a template.

E.g. 

    cp ec2_vars/sample.yml ec2_vars/webservers.yml
    vi ec2_vars/webservers.yml
    
After setting all variables, run it:

    ansible-playbook -vv -i localhost, -e "type=webservers" provision-ec2.yml
    
More info: [http://allandenot.com/devops/2015/01/31/provisioning-ec2-hosts-with-ansible.html](http://allandenot.com/devops/2015/01/31/provisioning-ec2-hosts-with-ansible.html)
