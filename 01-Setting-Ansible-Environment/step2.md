Installing Ansible Control Machine.

## Task

For the purpose of this demonstration, we will be installing Ansible on Ubuntu machine. If you are comfortable with other flavors, you can use the below link for reference to proceed with the installation in your VM-ware or other lab setup.

**[Ansible Installation Guide](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html).**

We will be using `apt` package manager to install Ansible on Ubuntu. To get the latest releases via `apt` you need to configure **[PPA](https://askubuntu.com/questions/4983/what-are-ppas-and-how-do-i-use-them/4990#4990)** on your machine. 

1.) Use the below command to updates the package lists for upgrades for packages that need upgrading, as well as new packages that have just come to the repositories. 

`sudo apt-get update`{{execute}}

2.) Run the below command which manage the repositories that you install software from (common).

`sudo apt-get install software-properties-common`{{execute}}

3.) Add the Ansible PPA to sources.list file

`sudo apt-add-repository ppa:ansible/ansible`{{execute}}

4.) After adding the PPA, you need to run the below command to update `apt` so that it can connect to the Ansible repository and pull the required files for installation.

`sudo apt-get update`{{execute}}

5.) Now you are ready to install Ansible by executing the below command:

`sudo apt-get install ansible`{{execute}}

6.) To verify if Ansible is installed correctly, you can run the below command which will reture the Ansible version details.

`ansible --version`{{execute}}

Hurray! You have successfully installed your Ansible Control Machine.