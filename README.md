# IT-Acedemy final project report
## Project's reporter: Sergei Sechkov
## Group number: md-sa2-22-22

## Description of application for deployment
- **Application:**  wp-project
- **Programming language:** PHP
- **Database:** Mariadb

## Pipeline. High Level Design
![scheme](thereissheme.png)

## Technologies which were used in project
**Orchestration:** K8s
**Automation tools:** Github Actions, ArgoCD, Ansible
**Other used technologies**: HELM, Docker, MariaDB
**SCM:** GitHub
**Notifications:** Slack

## CI/CD description
**General description:**

**Deployment:**
ArgoCD checks ArgoCD Apllication yaml on GitHub Repo by timer and upgrades all changed manifests to be the new helm chart version.

**Rollback:**
We can use ArgoCD for manual rollback to previous application version. External database contains all user data which will remain.

### Links
[Project Repository](https://github.com/frame0310/it-academy-project)
[DockerHub Registry](https://hub.docker.com/u/frame0310/IT-Academy-project/tags)
[Git Wordpress Docker library](https://github.com/docker-library/wordpress)