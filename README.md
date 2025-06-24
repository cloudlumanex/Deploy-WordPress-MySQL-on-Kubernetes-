# Deploy WordPress MySQL on Kubernetes
This project demonstrates how to deploy a scalable, modular two-tier web application WordPress and MySQL on Kubernetes, showcasing infrastructure as code, container orchestration, and service exposure using Kustomize for maintainable YAML management.

## 🧱 Architecture

- WordPress frontend
- MySQL backend
- Persistent storage for MySQL
- Kustomize for resource management


## 📁 Files

- `wordpress-deployment.yaml`: WordPress Deployment + Service
- `mysql-deployment.yaml`: MySQL Deployment + Service
- `kustomization.yaml`: Kustomize overlay


## 🔧 Key Problems Solved by the Project

| Problem                        | Solution                                                                                     |
|-------------------------------|----------------------------------------------------------------------------------------------|
| **Multi-tier application setup**  | Used Kubernetes Deployments and Services to orchestrate the frontend (WordPress) and backend (MySQL) containers. |
| **Manual and inconsistent setup** | Defined infrastructure using version-controlled YAML manifests, enabling reproducibility and automation. |
| **Lack of application portability** | Containerized both WordPress and MySQL, ensuring consistent behavior across local, cloud, and CI/CD environments. |
| **Configuration complexity**       | Leveraged **Kustomize** to organize, customize, and manage Kubernetes resources without duplicating YAML files. |
| **Local development constraints** | Used **Minikube** to simulate a cloud-like Kubernetes environment for local development and testing. |
| **Volatile data storage**         | Configured **PersistentVolumeClaims (PVCs)** to ensure MySQL data persists across pod restarts and is decoupled from containers. |


# DevOps Skills Demonstrated
Container orchestration: Running and scaling containers via Kubernetes

Declarative Infrastructure: Managing deployments using YAML

Service exposure: Exposing apps using NodePort or minikube service

Resource management: Using Kustomize to manage layered manifests

Troubleshooting: Diagnosing pod failures (ImagePullBackOff, etc.)

CI/CD potential: The YAML structure is CI/CD-ready (GitHub Actions or Jenkins integration)

# Real-World Relevance
This kind of setup mimics what DevOps engineers do in the real world for:

Deploying CMS platforms

Migrating legacy apps to Kubernetes

Automating infrastructure with IaC

Building development and testing environments quickly



![Image](https://github.com/user-attachments/assets/8b67a67b-6266-463b-b21c-4d1ce3ca50b9)
![Image](https://github.com/user-attachments/assets/7041bccd-40b0-40e4-af07-58995b4d1f90)
# Secret
![Image](https://github.com/user-attachments/assets/d3144025-bbab-4163-8b59-56ebc1160e1c)
# Mysql
![Image](https://github.com/user-attachments/assets/26d003c3-60cd-4f04-907d-fe42185beae9)
# wordpress.yaml
![Image](https://github.com/user-attachments/assets/79324368-eea9-4d38-916a-babb2995d414)
# pods
![Image](https://github.com/user-attachments/assets/ee7059ab-9fa8-49fb-b1c7-ceea75e91bcf)
# PVC
![Image](https://github.com/user-attachments/assets/3241cf92-3bbd-4e26-8f8c-ac8537242f2c)
# Secrets
![Image](https://github.com/user-attachments/assets/2258d1f4-1575-4e6e-883d-ce06cd9bd10e)
# Service
![Image](https://github.com/user-attachments/assets/7e3bf83b-cbb3-4bb4-86f5-2f0a191b1187)
