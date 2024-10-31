# CI/CD with Ansible Configuration Deploy

## Description
Ce projet vise à mettre en place un pipeline CI/CD à l'aide d'Ansible pour déployer des applications sur OpenShift et Kubernetes. Il contient des playbooks qui configurent l'environnement de déploiement, gèrent les secrets et effectuent les déploiements d'application.

## Prérequis
- Ansible installé sur votre machine
- Accès à OpenShift ou Kubernetes
- Docker installé

## Cloner le dépôt
Pour cloner ce dépôt, utilisez la commande suivante :
```bash
git clone https://github.com/achrefB2525/CI_CD_with_Ansible_Config-deploy.git
Ensuite, naviguez vers le répertoire du projet :

cd CI_CD_with_Ansible_Config-deploy
Branches
Pour utiliser la branche openshift :
bash
Copier le code
git checkout openshift
Pour utiliser la branche kubernetes :
git checkout kubernetes
Pour configurer le CI/CD, exécutez le playbook Configure-ci-cd.yml avec la commande suivante :


ansible-playbook -i inventory_file_path deploy-ci-cd/playbooks/Configure-ci-cd.yml
Pour déployer l'application, exécutez le playbook deploy-ci-cd.yml :


ansible-playbook -i inventory_file_path deploy-ci-cd/playbooks/deploy-ci-cd.yml
