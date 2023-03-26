## Vous trouverez un compte rendu des réponses de la partie 1 dans le dossier ansibleLabsTLC (nous n'avons pas réussi à faire la partie 2)

# demoAnsible

## Setup

- Install Virtualbox
- Install vagrant
- Install ansible
- Start the VMs using vagrant


```bash
git clone https://github.com/barais/demoAnsible
cd vagrant
vagant up
# Check that the VM are up
# Check that you can login using ssh (ssh vagrant@192.168.56.141 # password: vagrant)
```

## Demo 1

Run the playbook

```bash
ansible-playbook playbook.yml -i hosts
```

Try to access http://192.168.56.141/index.php

## Demo 2

- Kill the VMs and remove them.
- Use vagrant to recreate them from scratch

```bash
git clone https://github.com/barais/demoAnsible
cd vagrant
vagant up
# Check that the VM are up
# Check that you can login using ssh (ssh vagrant@192.168.56.141 # password: vagrant)
```

Run the playbook

```bash
ansible-playbook site.yml -i hosts
```

Try to access http://192.168.56.141/index.php
