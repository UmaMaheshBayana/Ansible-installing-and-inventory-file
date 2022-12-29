# Ansible-installing-and-inventory-file

1) Install Ansible on AWS Ec2 machine

```
sudo apt update
````
```
sudo apt install software-properties-common
````
```
sudo add-apt-repository --yes --update ppa:ansible/ansible
````
```
sudo apt install ansible
````

2) Create Hot Mahcines both Application and Database mahcine, and while creating mahcine, configure Ansible machine security group details to host mahcines security groups.

3) Connect to Ansible machine to configure Host machine details in inventory files to ping.
4) Create a sample directory
```
sudo mkdir testproject
````
```
cd testproject
````
```
sudo mkdir exercise1
````
```
cd exercise1
````
5) Create Inventory file.
```
sudo vim inventory
````
```
$HOST_MACHINE_NAME1 ansible_host=$PRIVATE_IP ansible_user=$USER_NAME ansible_ssh_private_key_file=$PEM.KEY
$HOST_MACHINE_NAME2 ansible_host=$PRIVATE_IP ansible_user=$USER_NAME ansible_ssh_private_key_file=$PEM.KEY
$DB_MACHINE_NAME ansible_host=$PRIVATE_IP ansible_user=$USER_NAME ansible_ssh_private_key_file=$PEM.KEY
````
6) Ping the server details.


