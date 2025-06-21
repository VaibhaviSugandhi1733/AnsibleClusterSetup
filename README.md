
# Ansible Cluster Setup using Docker & Kubernetes

This project demonstrates how to manually set up an Ansible cluster for automation testing using both Docker containers and Kubernetes Pods — **without relying on pre-built images**.

## 📦 Project Structure

```

AnsibleClusterSetup/
├── Ansible-Cluster-Setup-in-Docker/
│   └── (Dockerfiles, setup scripts, SSH config, inventory, etc.)
├── Ansible-Cluster-Setup-in-Kubernetes/
│   └── (K8s manifests, headless services, SSH, node setup, etc.)
└── README.md

````

## ⚙️ What’s Inside

### 1. Ansible Cluster in Docker
- Manual Dockerfile-based image creation using `ubuntu` or `centos`
- One control node (Ansible master) and multiple managed nodes
- SSH key-based authentication
- Static inventory configuration
- Testing with Ansible ad-hoc and playbooks

### 2. Ansible Cluster in Kubernetes
- Manual pod and service configuration (no Helm or pre-built charts)
- Uses headless services for pod-to-pod SSH
- Persistent pod names and role-based selectors
- Fully manual installation of Ansible and dependencies

---

## 🚀 How to Use

### Clone the Repo
```bash
git clone https://github.com/VaibhaviSugandhi1733/AnsibleClusterSetup.git
cd AnsibleClusterSetup
````

### Docker Setup

```bash
cd Ansible-Cluster-Setup-in-Docker
# Follow provided steps in README or scripts to build images and run containers
```

### Kubernetes Setup

```bash
cd Ansible-Cluster-Setup-in-Kubernetes
# Apply YAML files and configure SSH manually for Ansible control
```

---

## 🛠️ Tools Used

* **Ansible** (automation)
* **Docker** (container platform)
* **Kubernetes** (container orchestration)
* **Ubuntu / CentOS** base images (built from scratch)

---

## 🎯 Goals

* Learn Ansible internals by manually setting up clusters
* Avoid automation shortcuts like prebuilt images or Helm charts
* Practice real-world SSH, YAML, and networking setups

---

## 📌 Author

**Vaibhavi Sugandhi**
[GitHub Profile](https://github.com/VaibhaviSugandhi1733)

---

