# Automated Kubernetes Deployment of a ToDoList App

This project sets up a complete on-premises Kubernetes cluster, to automatically deploy a full-stack ToDoList application.

It demonstrates how to manage the entire lifecycle of a microservices-based application using modern DevOps tools like Ansible, Helm, and ArgoCD, from infrastructure provisioning to GitOps-based application deployment.

The ToDoList app used in this project was originally developed by me [here](https://github.com/Thybaau/todolist-app), and has been fully containerized and adapted for Kubernetes.

## Functionalities

This project demonstrates how to:

#### 🛠️ Using Ansible:

- Provision a kubeadm Kubernetes cluster from scratch.

- Install Helm and Helmfile.

- Install and configure ArgoCD using Helmfile for GitOps-based continuous delivery.

#### 📦 Using ArgoCD

- Automatically deploy a full-stack ToDoList application (frontend, backend, and PostgreSQL database) using Kubernetes manifests (Deployments, Services, ConfigMaps, NetworkPolicies).

- Secure sensitive data with SealedSecrets, enabling safe Git storage for Kubernetes secrets.

- Apply Kubernetes objects like ConfigMaps, Services, and NetworkPolicies to ensure modularity and security.


<!-- ### Built with

#### Server :
* [![Golang][Go]][Go-url]
* [![Nginx][Nginx]][Nginx-url]
#### Client:
* [![React][React.js]][React-url]
* [![Vite][Vite]][Vite-url]
* [![Tailwind CSS][Tailwind]][Tailwind-url]
#### Database :
* [![Postgre][Postgre]][Postgre-url]
#### Containerization :
* [![Docker][Docker]][Docker-url] -->

### Todolist functionalities

* Real time tasks list.
* Add new task, settings his content.
* Delete task, by clicking on red button to the right of each tasks.
* Edit task, by clicking on the pencil button to the right of each tasks.
* Check/uncheck task with checkbox button. This will validate and cross task.

### Upcoming features

- 🏗️ Configure ArgoCD to handle helmfiles

- 🏗️ Integrate Prometheus and Grafana with ArgoCD and helmfiles for application and cluster monitoring

- 🏗️ Add Loki for centralized log collection and visualization

## Getting Started

### Installation

1. If not already done, get a public SSH key.

2. Clone the repo via SSH
  ```sh
  git clone git@github.com:Thybaau/deploy-todolist-iac.git
  ```

3. Or you can clone it via HTTPS
  ```sh
  git clone https://github.com/Thybaau/deploy-todolist-iac.git
  ```



<!-- MARKDOWN LINKS & IMAGES -->

[issues-shield]: https://img.shields.io/github/issues/github_username/repo_name.svg?style=for-the-badge
[issues-url]: https://github.com/github_username/repo_name/issues

[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username

[Go]:     https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white
[Go-url]: https://go.dev/

[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/

[Vite]: https://img.shields.io/badge/Vite-B73BFE?style=for-the-badge&logo=vite&logoColor=FFD62E
[Vite-url]: https://vitejs.dev/

[Tailwind]: https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white
[Tailwind-url]: https://tailwindcss.com/

[Docker]: https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white
[Docker-url]: https://www.docker.com/

[Nginx]: https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white
[Nginx-url]: https://www.nginx.com/

[Postgre]: https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white
[Postgre-url]: https://www.postgresql.org/
