# ansible
ansible-playbook fedora-playbook.yml --ask-vault-pass

ansible-playbook -i inventory backup-server-playbook.yml -u admin --ask-pass

ansible-playbook -i inventory common-playbook.yml -u admin --ask-pass --ask-vault-pass

ansible-playbook -i inventory file-server-playbook.yml -u admin --ask-pass --ask-vault-pass

ansible-playbook -i inventory name-server-playbook.yml -u admin --ask-pass --ask-vault-pass

# added ssh-key

# manual
https://www.if-not-true-then-false.com/2015/fedora-nvidia-guide/
