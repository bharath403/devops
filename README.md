# This Terraform script will Provision EC2 instance, create new EC2 key pair and Security Group, Install Nginx and configure SSL

Run with a command like this:

```
terraform apply -var 'key_name={your_aws_key_name}' \
   -var 'public_key_path={location_of_your_key_in_your_local_machine}'
```

For example:

```
terraform apply -var 'key_name=mykey' -var 'public_key_path=/home/vagrant/.ssh/mykey1.pub'
```

#Automation of NGINX Config using Ansible

Run the Ansible playbook nginx.yml to configure NGINX like this:


for example:

```
ansible-playbook nginx.yml
``` 
