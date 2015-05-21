# playbook-ansible-pod
script playbook used to install and configure pod project

--------------------------------------------------------------------------------------------------------------------------------------------------------

PRESENTATION ANSIBLE

Ansible est un outil d'automatisation de tâches d'administration système. Il permet de configurer des machines, installer des logiciels, ou orchestrer des tâches plus avancées comme du déploiement continu ou de la mise à jour sans arrêt de service. Il s'appuie entièrement sur SSH pour la communication, et sur le langage Python pour l'exécution, ce qui en fait un outil quasi universel dans la mesure où il fonctionne sans agent à préinstaller et que SSH et Python sont des outils livrés en standard sur la plupart des serveurs.


Pour orchester les taches à faire sur un ou plusieurs serveurs, il faut créer des playbooks. Les playbooks sont des scripts utilisant le language YML. 

Nous avons, dans ce projet, développé des playbooks pour la gestion de la plateforme Pod : https://github.com/SemmLille/pod

Il y a 2 étapes pour mettre en place Pod sur un serveur : l'installation et la mise en production. 2 playbooks, installation.yml et Mise_en_production.yml font respectivement ce travail. 
Un troisieme playbook nommé "mise_a_jour_pod.yml" est présent pour la mise à jour d'une instance Pod.

---------------------------------------------------------------------------------------------------------------------------------------------------------

