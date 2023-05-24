ansible-playbook -i .vagrant/provisioners/ansible/inventory/vagrant_ansible_inventory playbooks/additional-packages-playbook.yml

ansible-galaxy install gantsign.oh-my-zsh

ansible-playbook -i .vagrant/provisioners/ansible/inventory/vagrant_ansible_inventory playbooks/oh-my-zsh.yml
