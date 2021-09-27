# Ansible AWX Inventory GIT Sourced

## Variables required

- `ansible_ssh_common_args='-o StrictHostKeyChecking=no'`: Disable host key checking in the lab 

Example host file

```yaml
[ios]

R1 ansible_host=192.168.1.93
R2 ansible_host=192.168.1.72

[ios:vars]

ansible_ssh_pass=cisco
ansible_user=cisco
ansible_network_os=ios
ansible_connection=network_cli
ansible_password=cisco
auth_pass=cisco

```

## AWX Configuration

AWX project configuration

![image](/assets/images/project.jpg)

AWX Inventory configuration

![image](/assets/images/inventory.jpg)
