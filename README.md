# playbook-ansible-pod
script playbook used to install and configure pod project

--------------------------------------------------------------------------------------------------------------------------------------------------------

PRESENTATION ANSIBLE

Ansible est un outil d'automatisation de tâches d'administration système. Il permet de configurer des machines, installer des logiciels, ou orchestrer des tâches plus avancées comme du déploiement continu ou de la mise à jour sans arrêt de service. Il s'appuie entièrement sur SSH pour la communication, et sur le langage Python pour l'exécution, ce qui en fait un outil quasi universel dans la mesure où il fonctionne sans agent à préinstaller et que SSH et Python sont des outils livrés en standard sur la plupart des serveurs.


Pour orchester les taches à faire sur un ou plusieurs serveurs, il faut créer des playbooks. Les playbooks sont des scripts utilisant le language YML. 

Nous avons, dans ce projet, développé des playbooks pour la gestion de la plateforme Pod : https://github.com/SemmLille/pod

Préalables
Pour l'environnement cible du déploiement (Debian Wheezy ou Jessie) :
* le package python-minimal (>= 2.7) est installé
* le package openssh-server est installé
* configurer le compte root sur la machine cible pour accepter la clé publique du client (/root/.ssh/autorized_keys)
Pour le client depuis lequel le playbook ansible est exécuté
* disposer d'un client ssh (ssh linux/Mac OS, PuTTY Windows)
* disposer d'un biclé ssh (ssh keygen -t rsa - b 2048 -C "mail@univ.fr" sous Linux/Mac OS)
* disposer d'un environnement ansible d'où sera exécuté le playbook
* référencer la machine cible dans la rubrique [dev_install] du fichier hosts à la racine des sources ansible


Adapter/Valider  les valeurs par défaut de l'installation : roles/dev_install/defaults/main.yml

Lancer le playbook ansible depuis le répertoire des sources livrées :
$ ansible-playbook -i hosts -site.yml

