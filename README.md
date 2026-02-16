# 🚀 DevSecOps GitOps Pipeline – Netflix Clone (Zero Cost Setup)

> A fully containerized end-to-end DevSecOps pipeline using GitHub Actions, Helm, ArgoCD, Kubernetes (Kind), Prometheus and Grafana — built completely free with no cloud cost.

---

## 📌 Project Overview

This project demonstrates a complete DevSecOps workflow:

* Secure CI with **SonarQube + Trivy**
* Multi-Architecture Docker builds (AMD64 + ARM64)
* GitOps-based CD using **ArgoCD**
* Kubernetes deployment using **Helm**
* Observability using **Prometheus + Grafana**
* Fully containerized local infrastructure (Kind cluster)
* Zero infrastructure cost

---

# 🏗 Architecture Diagram

(Add your architecture screenshot here)

<img width="2890" height="680" alt="diagram-export-16-02-2026-22_46_31" src="https://github.com/user-attachments/assets/44db6fec-b295-43a6-a136-0aeb079547d6" />

---

# 🔄 CI Pipeline (GitHub Actions)

### Includes:

* Code Checkout
* SonarQube Analysis
* Trivy Security Scan
* Multi-Arch Docker Build (buildx)
* DockerHub Push

📸 Screenshot:

<img width="795" height="713" alt="Screenshot 2026-02-16 at 11 49 15 PM" src="https://github.com/user-attachments/assets/b3e037d3-b73c-4e00-846e-9fe8e36ec839" />

---

# 📦 Container Registry

Docker images are pushed to:

DockerHub Repository:
`https://hub.docker.com/r/<your-username>/netflix`

Multi-architecture image support:

* linux/amd64
* linux/arm64

---

# 🚀 CD & GitOps (ArgoCD + Helm)

Deployment flow:

1. CD updates Helm `values.yaml`
2. Commit pushed to GitHub
3. ArgoCD detects change
4. Syncs application to Kubernetes
5. Helm renders manifests

📸 ArgoCD Screenshot:

<img width="804" height="706" alt="Screenshot 2026-02-16 at 11 50 21 PM" src="https://github.com/user-attachments/assets/e85b650f-a47d-48dc-ad60-4bd0b4d9932b" />

---

# ☸ Kubernetes Deployment (Kind Cluster)

Resources Deployed:

* Deployment
* ReplicaSet
* Netflix Pods (2 replicas)
* NodePort Service

📸 Kubernetes Screenshot:

<img width="1440" height="900" alt="Screenshot 2026-02-16 at 3 29 04 AM" src="https://github.com/user-attachments/assets/6f103300-8620-4057-8302-43080d234938" />

---

# 📊 Observability Layer

Monitoring Stack:

* Prometheus (Metrics Collection)
* Grafana (Visualization)

📸 Prometheus Screenshot:

<img width="1440" height="900" alt="Screenshot 2026-02-16 at 3 29 14 AM" src="https://github.com/user-attachments/assets/4200d464-2d60-4e7b-a691-aa8296190c48" />

📸 Grafana Dashboard:

<img width="1440" height="808" alt="Screenshot 2026-02-16 at 11 53 46 PM" src="https://github.com/user-attachments/assets/90b17d44-88fa-4733-bd52-3a57ad86fe8e" />

---

# 🔐 Security Integration

Security tools used:

| Tool           | Purpose                          |
| -------------- | -------------------------------- |
| SonarQube      | Code Quality & Static Analysis   |
| Trivy          | Container Vulnerability Scanning |
| GitHub Actions | Automated CI/CD                  |

Security-first approach:

* Scans run on every push to main
* Images scanned before deployment
* No manual intervention required

---

# 🧰 Tech Stack

* GitHub
* GitHub Actions
* Docker
* Docker Buildx
* Helm
* ArgoCD
* Kubernetes (Kind)
* Prometheus
* Grafana
* SonarQube
* Trivy

---

# 🖥 How to Run Locally

High-level steps:

```bash
# Create Kind cluster
kind create cluster

# Install ArgoCD
kubectl create namespace argocd

# Deploy monitoring stack
helm install monitoring ...

# Push code to trigger CI/CD
git push origin main
```

(You can customize this section based on your setup.)

---

# 💰 Cost

Total infrastructure cost: **₹0 / $0**

Everything runs locally using containers:

* Kind cluster
* SonarQube
* Prometheus
* Grafana
* ArgoCD

---

# 🎯 Key Highlights

✔ Fully automated DevSecOps pipeline
✔ GitOps-based deployment
✔ Multi-architecture Docker builds
✔ Security integrated in CI
✔ Observability enabled
✔ 100% containerized
✔ Zero cloud cost

---

# 👨‍💻 Author

Abhinay Yalla
DevSecOps Engineer

LinkedIn: (your link)

---

# 🔥 Extra Pro Tip

Create this folder structure in repo:

```
screenshots/
 ├── architecture.png
 ├── argocd.png
 ├── ci-pipeline.png
 ├── prometheus.png
 ├── grafana.png
 ├── k8s-pods.png
```

Keep screenshots:

* Clean
* Cropped
* Dark theme (looks modern)
* High resolution

---

