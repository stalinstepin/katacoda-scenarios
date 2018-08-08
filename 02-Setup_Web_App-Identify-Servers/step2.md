Creating inventory file and adding the hosts to manage the target machines using Ansible.

## Task

We need to create an inventory file so that we can add the hosts into that file to manage them via ansible. You can use the following file for reference.

Now that you have the inventory file configured, you need test a ping command to see if you are able to connect to them.

You can use the following ad-hoc command to test your connection to ansible:

`ansible <alias> -m ping -i <inventory_file>`{{execute}}

Great. You can see that you are able to establish a successful connection to both the hosts. 

Now its time for us to start writing some playbooks to setup Web Application on these hosts.

Gear up!!
