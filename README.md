# Installer Wordpress avec Ansible

## IP de l'host

Il faut avant toute chose préciser l'IP de note machine sur laquelle nous voulons procéder aux installations.
Pour cela depuis le dossier cloné : 
```
cd host_vars/
nano machine1.yml
```
Changer
```
ansible_host: xx.xx.xx.xx
```
par 

```
ansible_host: IP de votre machine
```
## Lancement du script

```
ansible-playbook wordpress_install.yml -i inventory.ini
```
