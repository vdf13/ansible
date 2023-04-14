# Projet:  Déploiement automatisé avec ANSIBLE
Utilisation de ansible pour préparer les machines virtuelles.

Installer ces machines en utilisant les playbooks qui font appel à des rôles défini.

## Roles
- *Création d'utilisateurs*
- *Mise à jour de OS selon la version de la machine:  centos ou debian*
- *Installation de Docker*


## Usage
- ansible-playbook -e @jenkins_add.json -e @password.json --tags user,install playbook.yaml
- *Choisir un des 2 fichiers [jenkins_add.json | jenkins_del.json]* 
  - *Le fichier contient les variables pour le playbook*
- *password.json*
  -*Le fichier contient les password, mis à part por ne pas diffuser sur le repository*
- *Les tags utilisés sont : user, install, delete, debian, centos, docker*

## A suivre
- en cours de développement: Role pour installer Kubernetes ...

- en cours de developpement : Role pour installer Jenkins ...
  - *Installation de Jenkins via une image docker*

