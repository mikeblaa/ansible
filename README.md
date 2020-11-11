# ansible
ansible-playbook fedora-playbook.yml --ask-vault-pass

ansible-playbook -i inventory backup-server-playbook.yml -u admin --ask-pass

ansible-playbook -i inventory common-playbook.yml -u admin --ask-pass --ask-vault-pass

ansible-playbook -i inventory file-server-playbook.yml -u admin --ask-pass --ask-vault-pass

ansible-playbook -i inventory name-server-playbook.yml -u admin --ask-pass --ask-vault-pass

# added ssh-key

# manual
Steps that there are no way to automate

## Install nVidia drivers on Fedora
https://www.if-not-true-then-false.com/2015/fedora-nvidia-guide/

## Install Fedora 32 on Raspberry Pi 3B+
From: https://fedoraproject.org/wiki/Architectures/ARM/Raspberry_Pi
arm-image-installer --image=Fedora-Minimal-32-1.6.aarch64.raw.xz --target=rpi3 --media=/dev/sda --resizefs