# 🚀 Docker Installation Automation with Ansible

Automate Docker installation and multi-container deployment on Ubuntu using Ansible.

---

# 📖 Project Overview

This project demonstrates how to automate Docker installation and container deployment using Ansible Roles.

A single Ansible playbook performs the following tasks:

- Update Ubuntu packages
- Install Docker Engine
- Install Docker Compose Plugin
- Enable Docker Service
- Add User to Docker Group
- Verify Docker Installation
- Deploy Nginx Container
- Deploy Redis Container
- Deploy PostgreSQL Container

---

# 🏗️ Architecture

```text
                Ubuntu Server
                       │
                Ansible Playbook
                       │
      ┌────────────────┼────────────────┐
      │                │                │
 Update Packages   Install Docker   Install Compose
                       │
               Enable Docker Service
                       │
                Verify Installation
                       │
               Deploy Containers
                       │
      ┌────────────────┼────────────────┐
      │                │                │
    Nginx           Redis         PostgreSQL
```

---

# 📂 Project Structure

```text
ansible-docker-automation/
├── ansible.cfg
├── docker-compose.yml
├── inventory/
├── group_vars/
├── playbooks/
├── roles/
│   ├── common/
│   ├── docker/
│   ├── docker_compose/
│   ├── verify/
│   └── containers/
├── README.md
└── LICENSE
```

---

# ⚙️ Technologies Used

- Ubuntu 24.04
- Ansible
- Docker
- Docker Compose
- Nginx
- Redis
- PostgreSQL
- Git
- GitHub

---

# 🚀 How to Run

Clone the repository:

```bash
git clone https://github.com/Bhabotos/ansible-docker-automation.git
```

Go to the project folder:

```bash
cd ansible-docker-automation
```

Run the playbook:

```bash
ansible-playbook playbooks/site.yml
```

---

# ✅ Verification

Check running containers:

```bash
docker ps
```

Check Docker version:

```bash
docker --version
```

Check Docker Compose:

```bash
docker compose version
```

---

# 🌐 Browser Test

Open your browser:

```
http://localhost
```

Expected Output:

```
Docker Nginx deployed successfully using Ansible
```

---

# 🗄️ PostgreSQL Test

```bash
docker exec -it postgres psql -U admin -d mydb
```

Inside PostgreSQL:

```sql
SELECT version();
```

---

# 🔴 Redis Test

```bash
docker exec -it redis redis-cli
```

```text
PING
PONG
```

---

# ✨ Features

- Role-based Ansible Project
- Docker Installation Automation
- Docker Compose Automation
- Multi-container Deployment
- Infrastructure as Code (IaC)
- Easy to Customize
- Beginner Friendly

---

# 📈 Future Improvements

- Ansible Vault
- Jinja2 Templates
- GitHub Actions
- Docker Swarm Support
- Kubernetes Deployment
- Multi-node Inventory

---

# 👨‍💻 Author

**Bhabotos Kumar**

- LinkedIn: https://www.linkedin.com/in/bhabotos-kumar-bd/
- GitHub: https://github.com/Bhabotos

---

# 📜 License

This project is licensed under the MIT License.
