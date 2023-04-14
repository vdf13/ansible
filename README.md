# Projet:  Déploiement automatisé avec ANSIBLE
Utilisation de ansible pour préparer les machines virtuelles.

Installer ces machines en utilisant les playbooks qui font appel à des rôles défini.

## Roles
- *Création d'utilisateurs*
- *Mise à jour de OS selon la version de la machine:  centos ou debian*
- *Installation de Docker*

## Usage
- ansible-playbook -e @jenkins_add.json -e @password.json --tags user,install playbook.yaml
- *[@jenkins_add.json | @jenkins_del.json]* 
  - * jenkins file containt data to set vars*
- *@password.json*
  - contain the password for the user
- *tags are : user, install, delete, debian, centos, docker*

- en cours de développement: Kubernetes ...

- en cours de developpement : Jenkins ...
- *Installation de Jenkins via une image docker*
