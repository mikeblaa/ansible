# README.md

## Ansible

Code snips for running the various playbooks in this repository

```bash
ansible-playbook fedora-playbook.yml --ask-vault-pass

ansible-playbook -i inventory backup-server-playbook.yml -u admin --ask-pass

ansible-playbook -i inventory common-playbook.yml -u admin --ask-pass --ask-vault-pass

ansible-playbook -i inventory file-server-playbook.yml -u admin --ask-pass --ask-vault-pass

ansible-playbook -i inventory name-server-playbook.yml -u admin --ask-pass --ask-vault-pass

ansible-playbook -i inventory pi-server-playbook.yml -u admin --ask-pass --ask-vault-pass
```

## Manual

Steps that there are no way to automate

### Install nVidia drivers on Fedora

<https://www.if-not-true-then-false.com/2015/fedora-nvidia-guide/>

### Install Fedora on Raspberry Pi 3B+

From: <https://docs.fedoraproject.org/en-US/quick-docs/raspberry-pi/>

1. Download a Fedora ARM image from the Fedora ARM website.
2. Install the arm-image-installer:3.  
  `$ dnf install -y arm-image-installer`
3. As the root user, write the Fedora ARM image to the microSD card:  
  `$ arm-image-installer --image=</path/to/fedora_image> --target=rpi3 --media=/dev/<sd_card_device> --resizefs`
