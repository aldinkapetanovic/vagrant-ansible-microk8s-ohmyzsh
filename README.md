ansible-playbook -i .vagrant/provisioners/ansible/inventory/vagrant_ansible_inventory playbooks/additional-packages-playbook.yml

ansible-galaxy install gantsign.oh-my-zsh

ansible-playbook -i .vagrant/provisioners/ansible/inventory/vagrant_ansible_inventory playbooks/oh-my-zsh.yml


(vagrant.exe wsl ansible)

vagrant_ansible_inventory


# Generated by Vagrant

microk8s-node-1 ansible_ssh_host=127.0.0.1 ansible_ssh_port=2222 ansible_ssh_user='vagrant' ansible_ssh_private_key_file='/home/ak/.vagrant.d/insecure_private_key'

microk8s-node-2 ansible_ssh_host=127.0.0.1 ansible_ssh_port=2200 ansible_ssh_user='vagrant' ansible_ssh_private_key_file='/home/ak/.vagrant.d/insecure_private_key'

microk8s-node-3 ansible_ssh_host=127.0.0.1 ansible_ssh_port=2201 ansible_ssh_user='vagrant' ansible_ssh_private_key_file='/home/ak/.vagrant.d/insecure_private_key'

