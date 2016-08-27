## VAGRANT
###Provisioning VM
`vagrant up`

### Access vm
`vagrant ssh` 

## ANSIBLE
`cd /vagrant/ansible`

### Edit vars.yml
Add your token and ssh key name in vars.yml. 
### Create machine
`ansible-playbook deploy.yml`

### Create machine
`ansible-playbook destroy.yml`
