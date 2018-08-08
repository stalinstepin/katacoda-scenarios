In this scenario, you will be using two target machines for Web Application and Database deployment/configurations.

## Task

Execute the command provided below to display the hosts file entry which has two hosts. 'host01' and 'host02' will be your target hosts whcih you will be using for this entire scenario.

`cat /etc/hosts | grep host`{{execute}}

As you can see, the above command displays the IP's of each host. With this information, you will now create an inventory file on the Ansible control machine from where you will be managing these target machines.

You can run the below command to confirm that you have Ansible installed and that this is your Ansible Control Machine.

`ansible --version`{{execute}} 

In the next step, you will be creating an inventory file and will be adding the hosts to the inventory file so that Ansible can manage these machines by running playbook against them.

