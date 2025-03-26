Debian 12.x Ansible
=========

Playbook Ansible permettant d'installer l'environnement de bureau Gnome et des applications utiles au quotidien pour une machine sous Debian 12 (Installation minimal).

Prérequis
------------
- Debian 12 mini installé (sans environnement de bureau)

- Il faut à minima git et ansible pour télécharger et lancer ce playbook

```
sudo apt install -y ansible git
```

Installation
---
Clone du projet :
```
git clone https://github.com/saiqo/debian-12-ansible.git
cd debian-12-ansible
```

Lancement du playbook :
```
sudo ansible-playbook -i inventory playbook.yml
```
> [!WARNING] 
> Le playbook doit être lancer avec l'utilisateur courant de la machine (pas root) mais avec les droits sudo.


Une fois le playbook terminé :
```
reboot
```

Customisation Bonus
---
Lancer l'application "Gestionnaire d'extension" et installer les applications suivantes :

- Blur my Shell
- Vitals
- Rounded Window Corners
