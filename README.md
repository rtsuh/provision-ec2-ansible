## Mysql Server Provisioning in EC2 using Ansible 

**OBJECTIVE:**

Create an Ansible playbook that takes in an input of a number, and launch/spin-up that number of AWS EC2 instances in the default VPC with MySQL installed and all instances updated.


**Usage:**

Create a variables file using *ec2_vars/sample.yml* as a template.

E.g. 

    cp ec2_vars/sample.yml ec2_vars/mysql-instances.yml
    vi ec2_vars/mysql-instances.yml
    
After setting all variables, run it:

    ansible-playbook -vv -e "type=mysql-instances" provision-ec2.yml
    
More info: [Mysql Server Provisioning in EC2 using Ansible](https://tinyurl.com/yd7rs8hb)
