# ansible
ansible-playbook fedora-playbook.yml --ask-vault-pass
ansible-playbook -i inventory fileserver-playbook.yml -u admin --ask-pass --ask-vault-pass


# added ssh-key
